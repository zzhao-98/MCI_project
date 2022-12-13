# Using the ZED 2 camera:
Sample website: https://www.stereolabs.com/docs/code-samples/

Record video: `python "svo_recording.py" my_svo_file.svo`<br>
Playback video: `python "svo_playback.py" svo_file.svo` <br>
Export video: 
```
svo_export.py A B C

Please use the following parameters from the command line:
 A - SVO file path (input) : "path/to/file.svo"
 B - AVI file path (output) or image sequence folder(output) : "path/to/output/file.avi" or "path/to/output/folder/"
 C - Export mode:  0=Export LEFT+RIGHT AVI.
				   1=Export LEFT+DEPTH_VIEW AVI.
				   2=Export LEFT+RIGHT image sequence.
				   3=Export LEFT+DEPTH_VIEW image sequence.
				   4=Export LEFT+DEPTH_16Bit image sequence.
 A and B need to end with '/' or '\'

Examples:
  (AVI LEFT+RIGHT)              export_svo.py "path/to/file.svo" "path/to/output/file.avi" 0
  (AVI LEFT+DEPTH)              export_svo.py "path/to/file.svo" "path/to/output/file.avi" 1
  (SEQUENCE LEFT+RIGHT)         export_svo.py "path/to/file.svo" "path/to/output/folder/" 2
  (SEQUENCE LEFT+DEPTH)         export_svo.py "path/to/file.svo" "path/to/output/folder/" 3
  (SEQUENCE LEFT+DEPTH_16Bit)   export_svo.py "path/to/file.svo" "path/to/output/folder/" 4

```