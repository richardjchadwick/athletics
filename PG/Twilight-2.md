## Procedures for Twilight #2 Meet

#### Restore a backup of Twilight #2 Meet
- Create a new folder for this meet e.g. C:\tfmeets6\2026-Twilight-2
- Make sure the backup file "Tfmm6BkupTwilightSeries-2-01.zip" file I emailed you is available on the laptop computer
- Choose "File/Restore" and select the option "Unzip, Copy database to a selected folder, and open this new database"
  - use the folder you created above
- <img width="734" height="226" alt="Hytek-Restore" src="https://github.com/user-attachments/assets/056939cb-d7aa-4c19-9cb4-31bfa2699326" />

### Hytek Run the Meet
- Go to "Run"
- Go to Interfaces/Update Start Lists and Use Change Data Location to change the location to folder created above eg. C:\tfmeets6\2026-Twilight-2
- <img width="401" height="298" alt="hytek-data-location" src="https://github.com/user-attachments/assets/a95542ee-a0b1-4ec7-8c3d-284d65cc6b51" />
- Then Select the Session Twilight and choose OK
- <img width="489" height="466" alt="Hytek-Update-Start-Lists" src="https://github.com/user-attachments/assets/1019030b-1c6a-4178-ad8b-21cb7b67b7cc" />
- This will create 3 files: lynx.sch, lynx.evt, lynx.ppl which Hytek uses to share information with Finishlynx.

### Finishlynx Equipment Setup

#### Indoor Equipment
- Cisco/Linksys Router
  - Connect power adapter
  - Plug into power bar 
- POE Injector
  - Plug into power bar
  - Use a short Ethernet cable to connect port labelled IN to any of ports 1-4 of Cisco/Linksys router
  - Connect the long Ethernet cable to the OUT port
  - The other end goes to the Camera via the Window
  - <img width="4032" height="3024" alt="POE" src="https://github.com/user-attachments/assets/21d839cb-543e-4e1b-bde9-3a7924ac2a7a" />
- Laptop
  - Plug into power bar
  - Connect short Ethernet cable from laptop to any of ports 1-4 of Cisco/Linksys router
  - <img width="4032" height="3024" alt="Laptop-Router" src="https://github.com/user-attachments/assets/fb790f3a-571a-4f82-adff-a7df4634061b" />
  
#### Outdoor Equipment
- Set up Tripod
  - Make sure the tripod is level using the levelling bubble on the tripod
  - Make sure the tripod head is level using the levelling bubble on the tripod head
  - Mount Camera on tripod
   - <img width="3024" height="4032" alt="Tripod" src="https://github.com/user-attachments/assets/7264567c-2551-43bf-830b-873e526cb820" />
- Connect RadioLynx (start system) to Camera
  - The 9-pin serial cable connects to the Serial port on the back of the camera
  - The red banana jack goes in the red 12 V output socket
  - Don't forget to attach the antenna
  - <img width="4032" height="3024" alt="CameraBack" src="https://github.com/user-attachments/assets/fb6ef756-8d9e-4db8-8abb-c66c7ff699d3" />- Connect the Connection Box
  - The long beige cable connects to the Connection Box port on the back of the camera
  - The other end of the cable goes into the end of the Connection Box
  - <img width="3024" height="4032" alt="ConnectionBox" src="https://github.com/user-attachments/assets/3a636152-1c81-4022-b9c0-cf7a63ea31de" />
- Connect wind gauge to the Connection Box
  - The 9-pin serial cable goes to the serial port
  - The red and black banana plugs go into the repsective red and black 12V Output jacks
  - The very long 50+m cable runs from the connection box to the Wind Gauge.
  - Locate the Wind Gauge outside the track at 50m from the finish line
    - It should be 1.2m from the ground to the sensors on the wind gauge.
    - That is eactly the width of 1 lane
    - Don't forget to level the wind gauge and ensure that the arrows are pointing in the direction of the running events
    - <img width="3024" height="4032" alt="WindGauge" src="https://github.com/user-attachments/assets/47dc2276-8880-4cb2-98ac-28682639fa41" />

### Finishlynx Tesing and Aligning of the Camera
- Launch Finishlynx on the Laptop
- Turn on the camera
- Within a few minutes the camera should show in the "Hardware Control Window"
- <img width="1091" height="255" alt="2d-alignment" src="https://github.com/user-attachments/assets/96b78260-155a-49a9-8ad4-5cbb54f04294" />
- I can't show a picture of 2d Alignment because my camera is too old and doesn't suport that feature
- The green line should be vertical.
- Try to get the green bar in 2d alignment mode on the front half of the white finish line (closest to lane numbers)
- Adjust Tilt and Zoom (middle ring of lens) so you can see the head of someone walking through lane 1 and the feet or at least legs of someone in lane 8.
- Adjust amount of light getting to the picture using the Iris control (inner ring of lens).
  - Increasing the frame rate will also reduce the amount of light
  - Decreasing the frame rate will increase the amount of light
  - But ideally for a 100m you want the rate at 1000fps -- for longer races 500-800 fps is good
- Test the RadioLynx
  - Make sure the transmitter has its antenna connected
  - Make sure the transmitter has the sensor attached. Green banana plug to green jack. Black banana plug to black jack.
  - Make sure the trasnmitter is ON.  Press and hold for 1-second the ON/OFF button (lower right)
  - Check the battery charge level. Quickly press and release the ON/OFF button. A full-day meet will use 5-10% of the battery.
  - Press the SIGNAL button.  Ensure that finishlynx receives the start signal
  - <img width="4032" height="3024" alt="RadioLynx" src="https://github.com/user-attachments/assets/fc2caaff-3b59-49e8-aa77-256f0774c3b5" />
- Update the Event Directory and Database Input and Output Directories
  - Choose Event Options and set the Event Dirdctory to the name of the folder for this meet eg. C:\tfmeets6\2026-Twilight-2
  - <img width="644" height="544" alt="Event-Options" src="https://github.com/user-attachments/assets/d73d3ea7-6d6f-4929-afc2-7220c87610fd" />
  - Under Options/Database set Input Directory and Output Directory to the same folder
- Start a new empty race for testing
  - <img width="1365" height="768" alt="NewFInishlynxEvent" src="https://github.com/user-attachments/assets/e45c1942-f737-4a74-b0c0-3066ac66f17a" />
  - Have the starter test the gun with the RadioLynx
  - The clock should start running
  - Enable Capture (Alt-T or click the Capture Icon)
  - <img width="344" height="145" alt="CaptureIcon" src="https://github.com/user-attachments/assets/6eeb495f-0825-42ac-8bb5-4bb828bea98f" />
  - Test capture by having someone run through the finish line in lanes 1, 4 and 8.
  - Turn off Capture (Alt-T or click the capture icon)
  - Assuming you have a reasonable photo you are ready to start the meet.

### Running the Meet
- Top of loop through all events
  - In Finishlynx do: 
    - Choose the first event or the next event
      - for the first event,  select Load Shedule and pick the first event from the menu
      - for subsequent events you can choose from below Load Schedule or you can just use Next Event (The down arrow)
      - <img width="1366" height="768" alt="finishlynx-choose-first-event" src="https://github.com/user-attachments/assets/a84d4e5e-f0e2-4b05-b460-7a29d0fb7801" />
    - Starter fires the gun
    - Verify the clock has started (or recall the race and try again)
    - Turn on capture (Alt-T or Capture Icon)
    - Evaluate finishers as they finish
    - <img width="1360" height="768" alt="finishlynx-evaluate" src="https://github.com/user-attachments/assets/94dac6e8-b7c0-4f28-86db-0755a850d080" />
    - Turn off capture (Alt-T or Capture Icon) after the last racer finishes
    - Double check you have results for all finishers
    - Save the event (Ctrl-S or File/Save and accept the name of the event by pressing Enter)
  - In Hytek Meet Manager (you can use Alt-TAB to cycle through applications running on the same computer)
    - Using the "Run"  Menu environment go to the event
    - Use "Get Times" or F3
    - This will import the results
    - If you have a printer connected you can use List and then print the results
- Go back to the Top of the loop and repeat for each event
