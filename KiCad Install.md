# KiCad Install instructions

## 1. Copy the files locally

Copy the `KiCad` folder wherever you like on your computer.

## 2. Install the Meadow F7 Micro board schema symbol

Use the `KiCad | Preferences | Manage Symbol Libraries...` command to manage the symbol library:

![symbol library manager](readme-images/kicad-Install/Image_01.png)

then select the global tab and click on the folder button:

![global libreries tab](readme-images/kicad-Install/Image_02.png)

navigate to your local `KiCad` folder, select the `KICAD_Meadow_EDA.lib` file and open it:

![select library](readme-images/kicad-Install/Image_03.png)

et voilà, the first step is completed:

![library list](readme-images/kicad-Install/Image_04.png)

You can now close the symbol libraries manager window.

## 3. Install the Meadow F7 Micro board footprint

You can use a similar approach to add the footprint to the footprint libraries manager, but I've found some issues that I've solved using the footprint editor, so here are the steps I suggest you to follow:

Open the footprint editor

![open footprint editor button](readme-images/kicad-Install/Image_05.png)

wait for the footprints to load... then use the `File | Add Library` command:

![add library command](readme-images/kicad-Install/Image_06.png)

select the `KICAD_Meadow_EDA.pretty` folder (yes, the folder represent a footprint library on KiCad):

![select library dialog](readme-images/kicad-Install/Image_07.png)

and confirm the `Global` choice:

![Library table selection dialog](readme-images/kicad-Install/Image_08.png)

Now the library is installed on KiCad with the Meadow F7 Micro footprint (double click on it to see it on the editor pane):

![footprint editor](readme-images/kicad-Install/Image_09.png)

Don't close the window as the next step start from here.

## 4. Install the Meadow F7 Micro board footprint 3D visual

If not already open, then open the the footprint editor

![open footprint editor button](readme-images/kicad-Install/Image_05.png)

double click on the `KICAD_Meadow_EDA` footprint from the `MeadowF7Micro_w_outline` library and then click on the `Footprint properties` icon:

![open footprint properties button](readme-images/kicad-Install/Image_10.png)

In the footprint properties window, first select the `3D Settings` tab. Please note that the preview shows only the PCB board with the footprint added on step 3, without any 3D representation of the Meadow F7 Micro board. Now click on the folder icon to add the 3D model:

![footprint properties dialog](readme-images/kicad-Install/Image_11.png)

Navigate to your local `KiCad` folder, select the `MeadowF7.wrl` file and wait until the model is shown in the right panel, then confirm with OK:

![add 3D model dialog](readme-images/kicad-Install/Image_12.png)

Now the 3D model is added to the footprint editor with the correct size and orientation and z-position (the model is placed on the PCB board):

![footprint properties dialog with added 3D model](readme-images/kicad-Install/Image_13.png)

now close the `Footprint Properties` window with the "Ok" button, and the `Footprint Editor`, obviously saving the changes.

![save changes button](readme-images/kicad-Install/Image_14.png)

## Conclusion

Now that you've installed the schema and footprint and added the 3D model to the footprint, you can use the Meadow F7 Micro board on your KiCad projects.

![3D model rendering example](readme-images/kicad-Install/Image_15.png)

Have fun!
