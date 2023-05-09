# *The Bowdoin Orient*'s Coverage of Vietnam Between 1955-75
### DCS 2500 Final Project

## Corpus
*The Bowdoin Orient* is the student-run newspaper of Bowdoin College, a private liberal arts college in Brunswick, Maine. It is one of the oldest continuously-published college newspapers in the United States, having been established in 1871. The paper is published weekly during the academic year and monthly during summers. *The Bowdoin Orient* covers news, features, opinions, and arts and entertainment related to the Bowdoin College community. The paper is staffed by Bowdoin students, who are responsible for reporting, writing, editing, designing, and publishing the paper. 

### Composition
**Publication:** *The Bowdoin Orient*

**Issue Range Searched:** `v.84 - 105`

**Date Range Searched:** `01/1955 - 12/1975`

**Issue Range Actual:** `v.91 - 105`

**Date Range Actual:** `10/12/1961 - 11/14/1975`

**Search Term:** `Vietnam` (match-case not enabled)

**Size:** TBD articles (currently 101)

**Language:** `en`

**Source:** [Bowdoin College Digital Commons](https://digitalcommons.bowdoin.edu/bowdoinorient/)

**Collection Method:** `Text extraction`, `manual collection`, `crowd-sourcing`

**Workflow & Quality Assurance:** 
Bowdoin's Digital Commons makes *The Bowdoin Orient* available in PDF files each representing a volume. The publishing cycle, on average, spanned April-April. Volumes 84-105 were downloaded for this project. Each volume was opened in either Adobe Acrobat where Optical Character Recognition (OCR) algorithms were used to query for the search term (`Vietnam`). Each article containing the search term was mined using crowd-sourced manual collection of the article's text (via copy & paste into a UTF-8 encoded .txt file).

<img src="images/1.png" width="750">

*Example of an article being queried for the search term. Source: pg. 35. v.91 PDF*

Each article was cross-checked for typos and punctuation errors. Due to poor archival and digitization quality of many of the volumes, the OCR algorithms often failed to work reliably. In these cases, manual transcription of the article text was used (via typing out each word by hand). In cases where words were not clearly discernible, as shown in the example below, a best guess was applied given the context of the preceding and following senteces. We acknolwedge that this is a subjective interpretation and leads to potential inaccuracy in the data, though luckily no article had its core meaning changed as a result of this.  

<img src="images/2.png" width="750">

*Example of poor archiving/digitization. Source: pg. 43, v.91 PDF*

The select terms `U.S`, `U.S.A.`, and `Viet Nam`, were re-written as `United States`, `United States of America`, and `Vietnam` respectively. Due to the physical constraints of print publication, historic newspapers such as *The Bowdoin Orient* used [abbreviations](https://web.archive.org/web/20220307224448/https://blog.newspapers.com/7-common-historical-newspaper-abbreviations-and-terms). Inconsistent terminology usage without standardization will result in measurements that are not wholly representative of the text.

### Data Structure

#### File Naming Convention: `VOL_MM-DD-YYYY_TITLE.txt`

`VOL` is a three digit integer representing the volume of the Orient that the article was found in. So, for example, volume XCVI (converted to 96) would be written as `096` in the filename.

`MM-DD-YYYY` is the date of publication of the volume the article was found in.

`TITLE` is the article title written in all caps, with periods substituting for spaces. All non-letter chacters are ommitted to ensure compatability, as there is no uniform way to handle special characters in file names across operating systems. So, if the article title is published in the Orient as "Sons and Daughters: The 'Berkeley' Bag," the title would be written as `"SONS.AND.DAUGHTERS.THE.BERKELEY.BAG"`

Between `VOL`, `MM-DD-YYYY`, and `TITLE`, underscores are used as delimiters.

All coming together, an article titled `"Sons and Daughters: The 'Berkeley' Bag"` published in `v.XCVI` on `April 21st, 1967` would be named `"096_04-21-1967_SONS.AND.DAUGHTERS.THE.BERKELEY.BAG"`


#### Article File Structure
Each article `.txt` file containts two pieces of useful information: `@TITLE=` and `@BODY=`

There is always a newline char `\n` between the `TITLE=` line and the rest of the document. Using the example from before, inside the file might look like this:

`@TITLE=Sons and Daughters: The "Berkeley" Bag`

`@BODY=Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit...`

#### Directory
The collection of articles are stored in `/articles/`. Nothing else is stored in this folder.