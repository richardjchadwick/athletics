# Notes for Chris Alward for Athletic Live

## AthleticLIVE Documetation
- the Athletic.net suport site, https://support.athletic.net/ has documentation on everything available from athletic.net
- documentation for AthleticLIVE, the part of the system we use is at https://support.athletic.net/category/mc9m1hkboq-athleticlive-timers
  - ignore anything that talks about ftp or uploading data. We use AthleticLIVE Local which automates uploads.
  - Whenever, the Hytek database is updated, AthleticLIVE Local uploads the changes. 

## Overview
- In order to easily use the AthleticLIVE suite of software with both FinishLynx and Hytek do the following:
  - Deignate a PRIMARY computer:
    - PRIMARY will be where FinishLynx is run
    - PRIMARY will also be where the Hytek Meet Database is installed
    - PRIMARY will also be where AthleticLive Local will be run
  - Designate a SECONDARY computer which will run Hytek
- For the CSG/Legion Trials and NB Provincial meet I have set up:
  - PRIMARY is SJTC2
  - SECONDARY is SJTC3

## Configuration of PRIMARY
- Set up 3 permanent virtual drives using SUBST
  - W:  ->  "C:\tfmeets6"
  - X:  ->  "C:\tfmeets6\Current Meet
  - Y:  ->  "C:\tfmeets6\Current Meet\lynx"


- Almost everything is done from the FinishLynx computer (SJTC2)
  - The Hytek database is to be located on this computer (SJTC2)
  - All copies of Hytek that access the meet **MUST** be in multi-user mode.
  - All files related to the current meet are located under c:\tfmeets\Current Meet\
    - The "Current Meet" should be X: (use subst on main computer or net use on hytek) see below.
    - The subdirectory lynx is where lynx.sch, lynx.evt and lynx.ppl will be read and written
    - The "lynx" subdirectory should be Y: (use subst or net use)
    - In addition all event files (.evn .i01 .i02 and i03) and lif files are written to Y:
    - There are various other subdiretories, but there use is optional
      - backups for Hytek backups
      - import for Trackie import files
      - reports for PDF reports from Hytek

  ### Set Up SJTC2
  - Configure X: 
  - [ ] Make sure the current Hytek database is installed and available on the X:\ Drive
