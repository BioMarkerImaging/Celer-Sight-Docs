# Tierpsy Guide
### 1) Start Tierpsy
Start tierpsy tracker by double clicking on the "Tierpsy Worm Tracker" desktop icon.

![Screenshot 2023-07-26 at 2 53 42 PM](https://github.com/BioMarkerImaging/Celer-Sight-Docs/assets/47221563/36387b7b-95f8-47b1-b7cc-dc19e1997604)

Current experiment location is : `D:\TierpsyTracker\Experiments`
Pre-generated parameters exist in  `D:\TierpsyTracker\Parameters`

### 2) Create Parameters
You can skip this step as I have already generate the parameters for you. If however the worms are not tracked properly you might have to adjust them.

1) Click "Set Parameters" on the Tierpsy Tracker introduction screen.
2) Click the "Video File" button and select 1 of your video files.
3) Go tot he "Background" tab on the top left, check "Substract Background" and select a large Background buffer size (Computes the background by averaging all of the images toger, more buffer equals better background but its more computationally expensive.
4) To back to the "Mask" tab and adjust min area and Max area to filter out small and large ROI. Adjust Theshold select the worm only and Dilation so that so that the ROI looks like the picture bellow
   ![image](https://github.com/BioMarkerImaging/Celer-Sight-Docs/assets/47221563/71e06ff5-744b-4b9b-a6c5-dddcd97a77a1)
5) Check "keep background data"
6) Click "Save Parameters" to save the the same location as the video file (or the location of your choosing)
7) Close the "set Parameters" window and go back to the introduction screen
### 3) Analysis
 1) In the introduction screen, click "Batch Processing Multiple Files".
 2) Click on the "Original Videos Dir" to select the folder under which your videos are located.
 3) Click on the "Parameters File" to select the parameter file provided to you (D:\TierpsyTracker\Parameters\default_parameters.json) or the custom one you generated on step 2)
 4) Adjust the "File Pattern to Include" to filter out videos for your analysis. If your videos end in ".wmv" then we can select all of the videos by using `*.wmv`. If however we only want the videos starting with `N2 we can do the following: `N2*.wmv`
 5) Make sure that there are no previous files in the "MaskedVideos" or in the "Results" directories, if there are, please delete them.
 6) Click on "START" and wait for the progress to finish.
 7) Once complete, close the "Analysis Progress" window and then close the "Batch Processing Multiple Files" window.
### 4) Inspect Tracking Result
 1) You can view each of the video file results by clicking on the Tierpsy Tracker Viewer button on the introduction screen.
 2) Then click on "Select Video File" and go to the "MaskedVideos" directory generated from the previous step. Select any life, all files will have the extention of ".hdf5".
 3) You can scrub through and inpect the video. for more details please take a look at the official tierpsy guide: https://github.com/ver228/tierpsy-tracker/blob/master/docs/HOWTO.md
 4) Click on the "PLOT" button after you select your desired feature to be measure on the drop down menu on the left (should be "speed" by default).
 5) Select "All Trajectories, Time Series" and write to csv.
