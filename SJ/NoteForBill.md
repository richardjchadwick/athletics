# Notes for Bill for Hytek
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
