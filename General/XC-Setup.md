##  General Configuration
- FinishLynx setting
  - From https://finishlynx.com/tag/cross-country/
    - Event/Results/TrackSelection = 0; 0=off 1=track selection (default) 2=ignore-out-of-bounds 3=new-results
    - Laptime/FillinTime=2 (always fill in time not just when hw=none)
    - Laptime/TotalLaps=1  OR Number of Laps
    - Database/Lif=Autosave=5
  - Configure Line Labels for both cameras
  - Camera Speed = 500fps
  - AutoCapture (leader=99  trailer=99  mintime=1.0
  - Scoreboards


## Days before meet

## Day before meet
- Ensure Generator and gerry can are topped up
- Ensure UPS is fully charged
- Ensure Trident Reader is fully charged
- Computer TCP/IP setup
  - 192.168.0.5/24 gw:192.168.0.1 (cell modem) OR use cell-phone via Wifi
- Mapping between RFID # Numbers and Bib #
  - In e:/Lynx/trident
  - Update mapping.sh
  - Run ./mapping.sh
  - Test the Mapping File
- Hytek
  - Make sure you have a workable Hytek File
  - location e:/tfmeets6/YYYY-XC/MeetName
  - Update Photofinish Start List for FinishLynx
  - Verify Lynx set to use profile IAT-XC
- FinishLynx
  - Use profile IAT-XC
  - Configure Meet Name
  - Configure directory options
    - Event Directory, Database Input and Output Directory
    - Laptime mapping file set

- Pack the Car


## At the Meet
- Set up Tent
- Set up table
- Set up generator (if required) OR run extension to AC power
- Set up UPS
- Set up mats
- Set up reader
- Set up cameras
- Set up tent/table/ups/computer 

### Day of Meet Checks
- Verify ping from computer to Trident Reader (192.168.0.101)
- Use Trident iTinyScore
  - Verify Computer and Trident Reader Date / Time agree
- Verify MAT RF Field is okay
  - Turn on Beep on All reads
  - Enable TX
  - Tune antennas
  - Verify field is knee or better height
 
### On Completion of the Meet
- Verify Live Results updated
- Post printable results (from Hytek)
- Post printable results (From Hytek) to trackie.com
- Post printable results (From Hytek) to live.athletics.net
- Email Hytek reports to Race Director
- Ensure Chips / Shoe Tags Collected

### After the Meet
- Send invoice to race director
