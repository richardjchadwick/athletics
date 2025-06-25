

- Almost everything is done from the FinishLynx computer (SJTC2)
  - The Hytek database is to be located on this computer (SJTC2)
  - All copies of Hytek that access the meet **MUST** be in multi-user mode.
  - All files related to the current meet are located under c:\tfmeets\Current Meet\
    - The "Current Meet" should be X: (use subst or net use) see below.
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
