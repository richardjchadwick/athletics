# Notes for Chris Alward and Bill MacMackin for NB Provincials
- If it shows up as a bullet point like this line then it is information to understand (the top sections below)
- [ ] if it shows up as a checklist like this line then it is something you have to do (the bottome sections below)

## For Bill and Importing Trackie and Setting up Hytek
- Some things are broken by using the standard import process.
- All of the below is "optional". It only fixes reltively minor issues we have lived with before.
  - Age Ups
    - Because Trackie is set up with Divisions but the meet file isn't, age-ups done in Trackie are lost
    - [ ] The solution is to run the script provided below and it will identify anyone who wants to age-up
    - [ ] The only way to deal with it in multi-age is to change their age
  - Accented Characters
    - The normal import screws up accented characters
    - [ ] The solution is to run the scripts provided below
  - Team Names
    - The normal import truncates team names in unusual places and shorter than necessary
    - [ ] The solution is to **manually** edit the long version of the team name in Hytek  
  - Masters age classes vs Other age classes
    - The normal import doesn't put Masters into the correct age-class because Hytek only allows one age-up date at a time
    - [ ] The solution is to run the script provided below AND ...
    - [ ] Purge previously imported athletes, entries, results (NOT TEAMS as you would undo your work above)
    - [ ] Set the Age-Up Date in Hytek to the first day of the meet
    - [ ] Import the file masters.txt produced by the script
    - [ ] Set the Age-up Date in Hytek to the last day of the year
    - [ ] Import the file ageclass.txt produced by the script

  ### To install the script above you have to:
  - Install MobaXterm from https://download.mobatek.net/2522025040602403/MobaXterm_Installer_v25.2.zip
  - Once MobaXterm is installed you have to launch MobaXterm and start
  - 
 

## AthleticLIVE Documentation
- The Athletic.net suport site, https://support.athletic.net/ has documentation on everything available from athletic.net
- Documentation for AthleticLIVE is at: https://support.athletic.net/category/mc9m1hkboq-athleticlive-timers
  - this is the ONLY part of Athetic.Net we use  
  - ignore anything that talks about ftp or uploading data from Hytek.
    - We use AthleticLIVE Local which automates that process:
      - when Hytek is updated, AthleticLIVE Local uploads the changes.

## Overview of What I Have Done.
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
  - X:  ->  "C:\tfmeets6\Current Meet
  - Y:  ->  "C:\tfmeets6\Current Meet\lynx"
- I have pre-installed a copy of the meet file frome June 25th
- I have set up the meet on AthleticLive as https://live.iatt.ca/meets/54634

- Almost everything is done from the PRIMARY computer (SJTC2)
  - The Hytek database is to be located on the PRIMARY computer (SJTC2)
  - All copies of Hytek that access the meet **MUST** be in multi-user mode.
  - All files related to the current meet are located under "C:\tfmeets6\Current Meet" which is alos X:\
    - Install the meet file on X:\  ( "C:\tfmeets6\Current Meet" )
    - The subdirectory lynx is where lynx.sch, lynx.evt and lynx.ppl will be read and written
    - The "lynx" subdirectory should be Y:\
    - In addition all event files (.evn .i01 .i02 and i03) and lif files are written to Y:|
    - There are various other subdiretories, but there use is optional
      - backups for Hytek backups
      - import for Trackie import files
      - reports for PDF reports from Hytek
      - logos, templates, etc.

### Configuration of SECONDARY
I have set up 
 
