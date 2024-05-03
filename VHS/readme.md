## Starting the Capture
* Open VirtualDub
* File -> Capture AVI...
* Device -> GV-USB2 Analogue Capture
* Turn on the VCR; you should see video from the VCR
* File -> Set capture file...
* Set your folder location and name your file
* Capture -> Capture video...
* Let the tape play as long as needed
* Capture -> Stop capture
* File -> Exit capture mode

## Deinterlacing the Video / Resizing For YouTube
* File -> Open video file...
* Select a raw video file
* Video -> Filters...
* Add...
* Deinterlace -> OK
    - Deinterlacing mode -> Interpolate using Yadif algorithm
    - Field order -> Double frame rate, top field first
        - IMPORTANT: Once you select this filter, go back to your side-by-side video view and step through the video frame by frame (using the left and right arrow keys).  If the video looks like people/animals/etc are moving back and forth instead of in the correct direction, choose "double frame rate, bottom field first"
* Add...
* Resize -> OK
    - Aspect Ratio: Disabled
    - New Size:
        - Absolute (pixels)
        - 960 x 720
    - Filter mode: Precise bicubic (A=-0.75)
    - OK
* Click OK until you return to the side-by-side view
* File -> Save As AVI...
* Set your file destination and let the export process complete
* Once finished: File -> Close video file

## Compressing the Video
* Open Handbrake
* Open Source -> File
* Choose your video file
* In the bottom section, choose Video
* Video Encoder: H.264 (x264)
* Framerate: 59.94
* Choose "Constant Framerate"
* Quality
    - Constant Quality
    - 15RF
* At the bottom of the screen, set your filename and destination
* In the top bar, select "Start Encode"
* Once the encode is finished, your conversion is complete
