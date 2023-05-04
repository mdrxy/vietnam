# *The Bowdoin Orient*'s Coverage of Vietnam Between 1955-75
### DCS 2500 Final Project

## Corpus

### Composition
**Publication:** *The Bowdoin Orient*

**Issue Range Searched:** v.84-105

**Date Range Searched:** 1955-1975

**Issue Range Actual:** TBD

**Date Range Actual:** TBD

**Search Criteria:** `Vietnam` (match-case not enabled)

**Size:** TBD (currently 101 articles)

**Language:** en

**Source:** [Bowdoin College Digital Commons](https://digitalcommons.bowdoin.edu/bowdoinorient@blank)

**Collection Method:** Text extraction, manual collection, crowd-sourcing

Each volume

**Quality Assurance:** 

### Data Structure

#### File Naming Convention
"VOL_MM-DD-YYYY_TITLE.txt"

VOL is a three digit integer to represent the volume of the Orient that the article was published in. So, for example, volume XCVI (translated to 96) would be written as 096 in the filename.

TITLE is the article title written in all caps, separated by periods. For the sake of cleanliness, all non-letter chacters are ommitted. So, if the article title as listed in the Orient is "Sons and Daughters: The "Berkeley" Bag" the title would be written as "SONS.AND.DAUGHTERS.THE.BERKELEY.BAG"

All coming together, an article titled "Sons and Daughters: The "Berkeley" Bag" published in volume XCVI on April 21st, 1967 would be named as "096_04-21-1967_SONS.AND.DAUGHTERS.THE.BERKELEY.BAG"


#### File Structure
Each article .txt file containts two pieces of useful information: "@TITLE=" and "@BODY="

There is always a newline char between the "@TITLE=" line and the rest of the document. Using the example from before, inside the file might look like this:

@TITLE=Sons and Daughters: The "Berkeley" Bag
@BODY=Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit...

That's it.