## How to use AthleticLOCAL for Live Results

### Assumptions
- You have a username/password for athleticlive
- X: is configured using subst to point to C:\tfmeets6\Current Meet
- Y: is configured using subst to point to C:\tfmeets6\Current Meet\lynx
- Files from previous meets should have been moved to another folder
- in X: the following subdirectories should exist
  ```
  mkdir backups docs imports logos lynx reports templates
  ```
  - backups -- stores hytek backups for this meet
  - docs -- stores techpackage, meet specific rules, etc
  - imports -- stores semicolon delimited files from trackie and related files
  - logos -- stores meet logo and/or additional team logos
  - reports -- team lists, schedules, meet programs, results and other PDF/HTML reports
  - templates -- save **copies** (use Save As...) of configured event files here to be used as templates
    
## Create an AthleticLive Meet
- [ ] Sign into your AthleticLive Dashboard at https://admin.athletic.live/
- Clone a previous meet
  - [ ] Choose a previous meet that is similar to the new meet e.g. previous year's meet or same location, same credit
  - [ ] Use the **View Admin Page** button
  - [ ] Choose Clone Meet
  - Proceed through the form changing what needs to be changed
    - The most common things that need changing are:
    - [ ] Meet Name
    - [ ] Abbreviated Meet Name
    - [ ] Meet Dates
    - [ ] You **MUST** check **Create Meet on AthleticNET**
    - [ ] Meet Credit
    - [ ] F.A.T Timing System should be **Finishlynx** for SJTC
    - [ ] Running Time System should be **Finishlynx** for SJTC
    - [ ] Email notifications are free
    - [ ] Text Message Notifications will incur additional charges based on how many messages are sent
    - [ ] Show Ads results in a price reduction with no ads that I have ever seen
    - [ ] Meet Management System should be **Hytek Database Connection** for SJTC
    - [ ] Hash Tag isn't important as I havent linked with Social Media
    - [ ] Image Export System should be **Finishlynx Image Export** if you want to publish photofinish and/or identlynx images
    - [ ] Require AthleticLOCAL should be **ON**
    - Once you're happy with your choices then select **Save Meet**
    - You can always modify these settings by choosing **Edit** from the meet's Admin panel.

## Enable Upload Protocols
- **Upload Protocols** must be **ON** in order to transfer data from Hytek and/or Finishlynx via AthleticLOCAL to https://live.iatt.ca
- AthleticNET will automatically enable upload protocols 2 days before the scheduled meet and turn them off 1 day after the meet.
- You can manually turn them on (or off) whenever you need from the **Admin Dashboard** by using the **Turn On Upload Protocols** button
  (see the right hand column of the screenshot below)<img width="1106" height="364" alt="UploadProtocols" src="https://github.com/user-attachments/assets/10886726-779c-4aa0-bcc8-4abf70458c5c" />

## Run AthleticLOCAL
- [ ] Make sure your Hytek Database is opened in **Multi-User Mode**
  - It will also work fine if your Hytek Database isn't opened at all :D
- AthletcLOCAL and AthleticSB icons are available on the SJTC laptop desktops
- Holding down the **Windows Key** and **D** is a quick way to access the desktop
- [ ] Launch **AthleticLOCAL**
- [ ] Sign into **AthleticLOCAL** using the same username/password that was used for the **Admin Page** above
- [ ] Select your meet
  - If your meet isn't available it either needs to be created or **Upload Protocols** is not on
- [ ] Configure Track Connection -- everything should be as below
<img width="1018" height="259" alt="track-connection" src="https://github.com/user-attachments/assets/a024b947-f5d0-4101-b85d-ea259b087e39" />

- [ ] Configure Image Export
  - SJTC1 is configured with Y: pointing to C:\tfmeets6\Current Meet\lynx
  - Turn on/off Generate Athlete Images and Generate Top Finisher Images as you desire
  - Window 1 is your left (or only) camera
    - I usually have this set to the outside camera for sprints
    - I have this set to the inside camera for distance events
  - Window 2 is your right camera
    - I usually have this set to the nside (reverse)  camera for sprints
    - I have this set to the Identilynx camera for distance events
  - If you only have one camera then use Window 1 for everything
<img width="1001" height="532" alt="images" src="https://github.com/user-attachments/assets/cf24b5aa-66f9-4b0c-9701-17addcbbf118" />

- [ ] Configure Hytek Database Connection
  - You have to select, type or paste the path to your the Hytek database (*.mdb) file
  - AthleticLOCAL will complain if your database is opened in **Single-User Mode**
  - Most other options are self-explanatory
  - Use **Performance Lists Only** if you haven't seeded but you want to show entries or you don't want to show seeded heats
<img width="989" height="616" alt="hytek" src="https://github.com/user-attachments/assets/f86221c5-4e0e-4e53-95d8-90d8c03d1fdb" />

- [ ] Configure path for AthleticField files (*.lff)
<img width="1010" height="207" alt="field" src="https://github.com/user-attachments/assets/5a6c8744-c2e2-47ba-8364-1e1d41e217ff" />

- Start AthleticLOCAL processes
- [ ] Use the **Start** button to start Hytek synchronization, Image Exports, etc
- [ ] Do **NOT** shutdown AthleticLOCAL -- either minimize or **Minimize to tray** 
<img width="361" height="216" alt="minimize" src="https://github.com/user-attachments/assets/68f326a0-945e-4719-ac1b-45ef765d650b" />



