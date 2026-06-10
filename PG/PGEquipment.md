### Pearlgate TFC Timing Equipment

- Vision Camera (SN: 50029 RAM: 256MB)
  - Timing Enabled 
  - Standard Resolution (1000fps 640 pixels)
  - Connection Box
  - POE Injector
- [Manual Camera Lens](https://www.finishlynx.com/product/c848-manual-lens/)
  - [Specs for OEM Computar](https://computarganz.s3.amazonaws.com/Computar+Active+Resources/H6Z0812+Spec.pdf) 
- Manfrotto Black Aluminum Geared Tripod
  - Manfrotto 410 Junior Geared Head 
- RadioLynx Wireless Start System
  - Transmitter w transducer (red N/O acoustic start sensor), transducer cable and antenna
  - Receiver w Antenna
- Wired Start
  - 100m XLR start cable on spool w transducer (white N/C acoustic start sensor) for wired starts
- Capture Plunger (9-pin Serial Only)
- [Lynx Ultrasonic Wind Gauge](https://www.finishlynx.com/product/ultrasonic-wind-gauge/)
  - Tripod for Wind Gauge
  - 50m XLR cable and connectors
  - XLR to 9-pin Serial adapater
- Electronumeric Race Clock Model: [607-9XLC-RD](https://raceclock.com/products/finishlynx-raceclocks/6-digit-ultra-bright-led-finishlynx-raceclocks/6-digit-ultra-bright-led-finishlynx/?attribute_6-digit-ultra-bright-led=Single+Sided%2C+9+Inch+tall+LEDs%2C+model+607-9XL-RD)
- See [manual])https://raceclock.com/wp-content/uploads/2018/05/Raceclock_XLC_Owners_Manual.pdf)
  - Could not find charger
  - Could not find data cable: Cable CA45-50
  - Speaker Mount/Tripod for Raceclock (not tested)
- 8-port TP-link network switch w POE  (Jeff found or replaced the power adapater)
- Laptop (I didn't get details other than runs Windows 10 and cannot be upgraded to Windows 11)
- Software
  - Hytek v. ???
    - Gold, Silver, Bronze: ???
    - Modules:
      - Photofinish
      - ??? 
  - Finishlynx v. 10.??
    - Plugins:
      - Auto-Capture Module (ACM)
      - Network COM Port  (NCP) (no longer needed as it is included for FREE with Finishlynx v 12.0 and later.)
      - ???
### Recommendations for Pearlgate Equipment
#### Upgrade Finishlynx to v13.10
- Though not required, it is a no cost upgrade and works even on my very old 2012 era backup laptop.
- Record your serial numbers in Help/About before upgrading
- [Download the latest Finishlynx](https://www.dropbox.com/scl/fi/6fb3zmxvg3pd72kou0a2v/FinishLynx-13.10.exe?rlkey=uy6ugavdajgwb4ioieo51gbm9&st=5ymkesv6&dl=1)
#### A USB-to-Serial connector for your Capture Plunger
- This is not required. Hwoever a capture button is useful even when you use the Auto Capture Module for:
  - Testing: easy to capture an image anytime to review image quality, check lane alignment
  - Laptiming: Put blank image for lead running when capturing all laps of a race to make it easy to identify laps.
- Your capture button is so old that the laptops back then had 9-pin serial connections but that hasn't been true for about 15 years
- Price: less than $CDN20
#### Purchase an Automatic Lens for your Vision Camera
- Using a manual lens for zoom, focus and especially iris control, outdoors could be very problematic.
  - The lighting due to cloud cover could change dramatically during a single race resulting in unreadable images at the finish line.
  - No one wants to learn that they don't have a time or placing after running a 1500m, 3000m, 5000m or 10000m!
- Finishlynx sells a [motorized (zoom, focus, and irs) lens for your Vision Camera](https://www.finishlynx.com/product/c848m-motorized-zoom-lens/)
  - The last price I saw was: $US619. Make sure that the cable that connect to the camera's remote control port is provided.
  - [OEM Specs for the above lens](https://computarganz.s3.amazonaws.com/Computar+Active+Resources/H6Z0812M+Spec.pdf) 
  - This lens allows zoom, focus, and iris to be controlled from the Finishlynx software
  - Finishlynx can be configured to automatically adjust the iris to keep consistent image quality even through wide ranges in lighting
#### Locate or Replace the missing charger and data cable for the Electronmerics Raceclock
- Before you do purchase anything verify the clock works.
  - It looks 100% new but you never know. 
  - Hopefully the battery has enough charge to verify that the clock turns on and works using manual controls.
  s- I have provided the part numbers for the mising pieces above as part of the eqipment list.
#### Investigate Wireless Solution for Wind Gauge and/or Race Clock
- A quick check of the track showed that there is power inside the track but I didn't see any network or serial connection
  - There is a utility cabinet that I couldn't open at the same location as power. There *may* be network or serial connections inside
  - I didn't see anywhere inside the timing hut where connections would terminate
- The wind gauge belongs 50m from the finish line 1-2m inside the track
  - The only way to connect the Wind Gauge currently is via a 50m hard-wired cable on the outside of the track
- Ideally the race clock would be positioned past the finish line on the inside of the track
- Two components would be required
  - [A SeriaLynx Serial-to-Ethernet Adapter](https://www.finishlynx.com/product/serialynx-serial-to-ethernet-adapter/)
    - Price: US$629
  - A wireless router or access point for the timing hut
    - Almost anything, including the Cisco/Linksys Wireless router I left in St John's
    - Price: less than $CDN150
