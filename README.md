# JTAG-adaptor
An adaptor from standard huge 20-pin ARM JTAG to a more compact format on the OBC. 

Getting started:
— -

- Clone this repo.
- Run `git submodule init` in the JTAG-adaptor directory, 
- Run `git submodule update`

Open the project in KiCAD. 

- In EESchema, go to Preferences > Component Libraries

- “Add" a user defined search path (bottom section of the window), select the KiCad-Lib directory in the JTAG-adaptor directory.
- “Add" component library files and select the SFUSat.lib file within the KiCad-Lib folder (top section of the window)
- Press ok.

Note: issues may arise when using relative paths. Select absolute paths by choosing "No" when asked if you want to use a relative path.

- Exit back to the KiCad home window and go to Pcbnew > Preferences > Footprint Libraries Manager > "Project Specific Libraries” tab:

- Click “Append Library"
- Enter the following information:
`Nickname: SFUSat`
`Library Path: ${KIPRJMOD}/KiCad-Lib/SFUSat.pretty`
