# Notes for Chris Alward for NB Provincials
- If it shows up as a bullet point like this line then it is information to understand (the top sections below)
- [ ] if it shows up as a checklist like this line then it is something you have to do (the bottome sections below)  

## AthleticLIVE Documentation
- The Athletic.net suport site, https://support.athletic.net/ has documentation on everything available from athletic.net
- Documentation for AthleticLIVE is at: https://support.athletic.net/category/mc9m1hkboq-athleticlive-timers
  - this is the ONLY part of Athetic.Net we use  
  - ignore anything that talks about ftp or uploading data from Hytek.
    - We use AthleticLIVE Local which automates that process:
      - when Hytek is updated, AthleticLIVE Local uploads the changes.

## Overview of What I Have Done for Running AthleticLive
- In order to easily use the AthleticLIVE suite of software with both FinishLynx and Hytek I did the following:
  - Deignated a PRIMARY computer:
    - PRIMARY will be where FinishLynx is run
    - PRIMARY will also be where the Hytek Meet Database is installed
    - PRIMARY will also be where AthleticLive Local will be run
  - Designated a SECONDARY computer which will run Hytek
- For the CSG/Legion Trials and NB Provincial meet I have designated:
  - PRIMARY is SJTC2
  - SECONDARY is SJTC3

### Configuration of PRIMARY
- I have set up 3 permanent virtual drives using SUBST 
  - W:  ->  "C:\tfmeets6"
  - X:  ->  "C:\tfmeets6\CurrentMeet
  - Y:  ->  "C:\tfmeets6\CurrentMeet\lynx"
- I have shared "C:\tfmeets6\"
- I have pre-installed a copy of the meet file frome June 25th
- I have set up the meet on AthleticLive as https://live.iatt.ca/meets/54634

- Almost everything is done from the PRIMARY computer (SJTC2)
  - The Hytek database is to be located on the PRIMARY computer (SJTC2)
  - All copies of Hytek that access the meet **MUST** be in multi-user mode.
  - All files related to the current meet are located under "C:\tfmeets6\CurrentMeet" which is alos X:\
    - Install the meet file on X:\  ( "C:\tfmeets6\CurrentMeet" )
    - The subdirectory lynx is where lynx.sch, lynx.evt and lynx.ppl will be read and written
    - The "lynx" subdirectory should be Y:\
    - In addition all event files (.evn .i01 .i02 and i03) and lif files are written to Y:|
    - There are various other subdiretories, but there use is optional
      - backups for Hytek backups
      - import for Trackie import files
      - reports for PDF reports from Hytek
      - logos, templates, etc.

### Configuration of SECONDARY
- I have used persistent net use to map
  - W:  ->  "\\LAPTOP-SJTC2\tfmeets\" 
  - X:  ->  "\\LAPTOP-JTC2\tfmeets6\CurrentMeet"
  - Y:  ->  "\\LAPTOP-SJTC2\tfmeets\CurrentMeet\lynx"

    - If you need to make a change in Hytek that requires single user mode then:
      - Stop AthleticLIVE Local first (see below)
      - Do your single user activity
      - Start AthleticLIVE Local (see below)

## What Chris/Bill need to do to run FinishLynx / Hytek / AthleticLive
- [ ] Ethernet Hub set up (Use Bill's Hub)
  - [ ] Network cable to cameras should be attached
  - [ ] Power ON Hub
- [ ] PRIMARY initial set up 
  - [ ] Connect SJTTC2 Ethernet Dongle to SJTC2  (closest USB port to front)
  - [ ] Connect SJTC2 Ethernet to Hub
  - [ ] Power SJTC2 ON
  - [ ] Login using PIN
  - [ ] Verify W: X: Y: subst mappings - type **subst** in a cmd window
  - [ ] Start Hytek in "Single User Mode" as "Admin"
    - [ ] Make sure you are using the database "C:\tfmeets6\CurrentMeet\2025 NBCHamps-CSG-Legions.mdb"
    - [ ] Restore the latest backup
    - [ ] Change to Multi-User mode: "File /  Open in Multi-User Mode" OR Close Hytek
- [ ] SECONDARY set up
  - [ ] Connect SJTC3 Ethernet Dongle to SJTC3 (closest USB port to front) - This is SECONDARY
  - [ ] Connect SJTC3 Ethernet to Hub
  - [ ] Power SJTC3 ON
  - [ ] Login Using PIN
  - [ ] Verify W: X: Y: net use mappings - type **net use** in a cmd window OR use FileManager
  - [ ] Start Hytek
    - [ ] Should automatically open the NB Provincial Meet
    - [ ] Sign into Hytek as "Run1" in Multi-User mode
    - [ ] Test printing (since I had no way to test printing)
  - [ ] At this point the Hytek operator can do whatever they need for the meet
 - [ ] PRIMARY set up continues
   - [ ] Set up AtheticLIVE
     - [ ] Make sure you have Internet access can you get to https://www.anb.ca ?
       - If my Eduroam didn't automatically login to WIFI (it should), you will have to tether a smartphone
       - Don't waste your time trying to use UNB Guest -- it will NOT work!
     - [ ] Start AthleticLive Local -- there is an icon on the desktop
       - If it says "WARNING: Unable to connect to the internet."
         - [ ] Verify you do have Internet
         - [ ] Close the AthleticLive Window
         - [ ] Start AthleticLive Local again
      - If it says "Welcome to AthleticLIVE Local version 3.9.25!" then:
        - [ ] DO NOT CLOSE that window.  Minimizie it!
        - [ ] In Chrome go to  http://localhost:8150  this is the interface to AthleticLIVE Local
          - If prompted for my username (email) and password. See the file Username-Passwords.txt on the Desktop.
        - [ ] Click the "Choose Active Meet" button
        - [ ] For Meet Select "NBProv-CSG-Legion - $54634"
        - [ ] For Hytek Database enter (include the quotes): "X:\2025 NBChamps-CSG-Legions.mdb"
          - you can also use File Manager to navigate to that file and use the "Copy as Path" to paste it.
        - [ ] Ensure "Enable Automatic Sync" is checked
        - [ ] The rest of the options are self-explanatory and shouldn't need to be changed.
        - [ ] Scroll to the bottom of the page and Click "Submit"
        - [ ] Verify you have a Green Highlighted "Can Connect to Hytek Database" box on the webpage now.
          - [ ] If not, you have either the wrong database path OR someone has it open in Single-User Mode.
        - At this point the database will sync to Athletic Live from now on.
        - There will be two links under the Green Highlighted "Can Connect to Hytek Database" box
          - [ ] One is to the Admin page for the meet - Open it
          - [ ] One is to the pages that everyone sees - Open it
          - [ ] Use these to ensure eveything is working.
          - [ ] If you want to anything more READ the DOCUMENTATION!
   - [ ] Set Up Hytek
     - [ ] Connect Capture Button to USB port
     - [ ] Start FinishLynx
     - [ ] Verify that you are using the "CSG" Profile"Can Connect to Hytek Database" box
       - If not you can change to the "CSG" Profile under Options / General Profile
       - Finishlynx requires a restart in order to change Profiles
     - [ ] Do the rest of your camera set up.
       - Scoreboards should all just work as they are defined in the "CSG" Profile 
        - Wind Gauge should work as long as it is connected properly
   - [ ] Optionally, Start Hytek as "Admin" in Multi-User Mode (only if you think you will need it).
     - If the Hytek operator is busy entering field results, then I will use Hytek to "Get Times"
        

## What Chris/Bill need to do to shutdown AthleticLive
- [ ] From the webpage http://localhost:8150 my email address will be in the top right corner
- [ ] Click on it and choose "Shutdown"
