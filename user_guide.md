# Celer Sight AI (User Guide)

## Instalation

1) Download the installer from the url:
   1) Go to: http://147.52.41.10:1080/repository/installers/
   2) Click on the available installer (`Celer Sight Installer beta.exe`)
   3) On the following warning `This type of file can harm your computer. Do you want to keep Celer Sight Installer.exe anyway`, press `Keep`. This warning is a false positive because this installed has not yet publickly been release yet.
   4) If any other warnings appear, please follow suit and ignore them or proceed. Celer Sight is an open source software and all of its code is available for everyone to look, modify and use at `https://github.com/BioMarkerImaging/celer_sight_ai`
2) Installer Celer Sight:
   1) If there is an old version of `Celer Sight AI` make sure to uninstall that first by going into Windows `Add or remove programs` from the search bar, then Click on the three dots on the `Celer Sight AI version XXX` and click uninstall.
   2) Processed by installing Celer Sight normally: Double click on the `celer_sight_installer.exe` (takes around 5-10 seconds to open).
   3) Make sure that the `Create a dsketop shortcut` button is clicked and click `Next`.
   4) Next, on the `Ready to Install` page click `Install` (should take around 5 minutes).
   5) Click `Finish`
3) Celer Sight AI will open automatically. If there are any updates, celer sight will download them, and restart celer sight to apply them (If that happens please wait for Celer Sight to restart by itself)

## Shortcuts

##### Zooming and panning
- Zoom in: `Control` + `scroll wheel up`
- Zoom out: `Control` + `scroll wheel down`
- Pan left or right: `Alt` + `Scroll wheel up / down`
- Pan up or down: `Scroll wheel up / down`
- Free hand pan: `Spacebar` + `Hold mouse click` and drag around

##### Tools
- Selection: `Q`
- Magic Box ROI generator : `F`
- Polygon ROI: `2`
- Brush Move: `3`

## Analysis Workflow

1) Import images by Drag & Drop on the center of Celer Sight (The main viewer were the image is shown)
2) Click on the `Get ROI (AI)` button on the top left of the UI under the `Workflow` section. Automated ROI generation has now started.
3) By clicking on the images its possible to refine the ROI's while the rest of the ROI are still generated. By using the Selection, Polygon, and the other tools provided, you can refine the ROIs that have been generated so far.
4) Once the ROI generation has been completed a pop up window with the title of `Success` should be displayed with the text `AI ROI generation complete.` . Once this window is displayed, all images have been proccessed by the automatic ROI generator. Click `ok` and inspect all of your images to make sure that no bad or missed ROI has been generated.
5) Click on the `Analyze` button and wait for the analysis to come to comletion. Once the analysis is complete after a few seconds the interface will switch automatically the the `Data` tab where you can view your results for ever channel and analysis type and copy them as comma or dot as a separator.
