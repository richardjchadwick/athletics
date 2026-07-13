# Meet Laptop Configuration
- Finishlynx Laptop has everything on it. I use a permanent SUBST command set via Windows Registry
  - Finishlynx
  - Hytek Meet Manager (must be run in multiuser mode)
  - The Hytek Meet Database is in X:\  (X: is SUBST to C:\tfmeets6\Current Meet
  - lynx.sch, lynx.evt, lynx.ppl *.lif, *.evn *.iXX go in Y:\  (which is the same as X:\lynx)
  - Hytek is configured so that all lynx files are read from Y:\
  - Finishlynx is configured to:
    - Save Events to Y:\  (Options/Event/Event Directory)
    - Database Input and Output Directories are set o Y:\  (Options/Database/Input Directory and Options/Database/Output Directory)
    - Use a Profile specific to the Venue (SJFH, CGS, Moncton, CEPS, etc)
      - this configures scoreboards and other things that are specific to the Venue
  - Athletic Live suite: AthleticLOCAL, AthleticSB, AthleticField
    - AthelticLOCAL uses the Hytek Database Connection / MS Access Engine that reads results from the HYtek Database automatically

- Hytek Laptop also has eveything installed. Drives X: and Y: are mapped so they correspond to the locations for X: and Y: above
  - Hytek Meet Manager (must be run in multiuser mode)
  - Finishlynx (configured to not look for cameras)
    - Can be used to re-evaluate a previous race
  - AthleticLOCAL, AthleticSB, AthleticField are installed but not typically used.

- Others
  - A second Hytek Laptop
  - Scoreboard Computer for streaming or local scoreboard support (eg. SJFH Projector Results)

# Preparing for a meet timeline
The timeline below is an overview. Follow links for more details.

## No less than two weeks before the meet
- [ ] Prepare techical package for meet
- [ ] Check Supplies (bibs, hip numbers, printer paper, printer toner, duct tape, masking tape)
- [ ] Setup Trackie registration
- [ ] Configure Hytek Meet Manager to match Trackie
- [ ] Preliminary setup of Live Results

## Week before the meet
- [ ] Ensure radios (walkie-talkies) are charged
- [ ] Ensure RadioLynx transmitter(s) are charged to more than 40%
- [ ] Perform daily download, import and verification of registrations
- [ ] Prepare preliminary schedule of events in Hytek
- [ ] Check Supplies (bibs, hip numbers, printer paper, printer toner, duct tape, masking tape, white gaffer's tape, black gaffer's tape, electrical tape)

## Two days before meet (close of early registration)
- [ ] Laptop security and application updates
  - [ ] Windows Updates
  - [ ] Hytek Updates
  - [ ] Finishlynx Updates
  - [ ] AthleticLive Updates (AthleticLOCAL, AthleticSB, AthleticField (autoupdates on tables and phones))
- [ ] Ensure Network between Hytek and Finishlynx laptopns is working
- [ ] Configure Hytek for the site-specific printer to be used.  (Set Up/Report Preference)
- [ ] Suspend Windows updates for 1 week
- [ ] Prepare detailed schedule of events in Hytek
- [ ] Synchronize Hytek with live results (post schedule and performance lists)

## Day before meet (close of late registration)
- [ ] Do final download, import and verification of registrations
- [ ] Do final seeding
- [ ] Ensure everything is synced with Athletic Live
- [ ] Update schedule of events if necessary
- [ ] Backup Hytek Database
- [ ] Ensure latest Hytek Meet Database is in place on Finishlynx laptop
 
## Day of meet
- [ ] Set up Timing Booth 
  - [ ] Network Switch plug in and power on
  - [ ] Printer
  - [ ] FinishLynx Laptop
    - [ ] Connect Power Cable
    - [ ] Plug in Capture Plunger
    - [ ] Connect Network Cable to Network Switch
    - [ ] Turn ON the power
    - [ ] Checks
      - [ ] Check Ethernet link on switch and laptop
  - [ ] Hytek Laptop
    - [ ] Connect Power Cable
    - [ ] Connect Network Cable to Network Switch
    - [ ] Connect Printer (is USB printer)
    - [ ] Turn ON the power
    - [ ] Check
      - [ ] Check Ethernet link on switch and laptop
      - [ ] Start Hytek Meet Manager
      - [ ] Verify you can Open the Meet Database from X:\ in multi-user mode
      - [ ] Verify you can print to the printer
-  [ ] Camera Setup
  - [ ] Set up Primary Camera
  - [ ] Set up Secondary Capture
  - [ ] Set up Identilynx Camera
