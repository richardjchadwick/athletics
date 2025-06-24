# Trackie Registration Configuration for NB Track and Field Meets

## Overview
As of April 2024, NB Track and Field Meets almost exclusvley use:
- Trackie Registration for input of entries and collection of fees
- Hytek Meet Manager for Meet Management including, definition of events, management of entries, seeding of events, printing and publishing of results
- Finishlynx for Photofinish results generation
- AthleticLive for online display of entries, performance lists, seeded events, results records, team scores etc

## Objectives
- To define "best methods" for configuring Trackie Registration for NB Track and Field Meets for easy import into Hytel Meet Manager.
- To provide an easy to use interface for coaches, parents and athletes for submitting entries
- To provide an easy, error-free way to import entries from Trackie into Hytek

## Assumptions
- Most NB meets do not use Divisions
  - Because of the small number of participants in age-class meets, there tends to be too few athletes per division.
    - we have optied to run events as "all-comers" events but use Hytek's Multi-Age Feature (ANB pays for this option) to combine events and split results by age division.
  - exceptions are NBIAA High School Meets, Jeux de l'Acadie, and Middle School Meets which have predefined age or grade divisions and enough athletes per division

## Trackie Configuration and Hytek Configuration Should Match
It is important to understand how the import process between Trackie and Hytek works, and how this process changes depending on configuration options.
The import process depends on a text file which contains several record types e.g. I - athlete info, D - event entry details.
Each record type has a predefined set of columns e.g.  FirstName; LastName; Birthdate; Club; Event; Seed; Division, etc (there are lots more)

- If your Hytek Meet Type Is Standard i.e. no Divisions, then matching between Trackie and Hytek will be based on Event-Age (birthdate is used to calulate age)
- If your Hytek Meet Type is Divisions by Event, then Matching between Trackie and Hytek will be based on Event and Division
- I am ignoring Divions by Team, Division by Entry etc. as we don't use them 

## Common Mismatch Problems
- No divisions defined in Hytek
   - Any information provided by Trackie re: Divisions is completely ignored.
    - If an athletes has been aged-up in Trackie, by using Divisions, that information is lost with the pursuing complaints that the athlete had been entered into the higher age category.
    - If there are online entries for SO, Para and able-bodied athletes then all athletes will end up in the first matching Event-Age which is NOT what is intended
      - One way to avoid this put SO, Para Ambulatory, Para Wheelchair into their own divisions


