# *The Bowdoin Orient*'s Reporting on Vietnam Between 1955-75
### DCS 2500 Final Project - Daugherty - README

***

## Context

I'm currently enrolled in HIST 2019: The Transatlantic Sixties and Seventies. As a result, I have spent a lot of time surveying the key themes, events, and attitudes that defined the period. In a true liberal arts nature, I am interested in connecting this to what I've been learning in DCS 2500: Digital Text Analysis by exploring *The Bowdoin Orient*'s reporting on the Vietnam War, an event that, in many ways, defined the era: the war was a catalyst that sparked widespread protests and political activism across college campuses worldwide, at levels never seen previously.

As a student publication, *The Bowdoin Orient*'s coverage of the Vietnam War likely reflected the attitudes and opinions of the Bowdoin student community towards the conflict. By examining its commentary on the war, I hope to gain insights into the perspectives and priorities of the Bowdoin community during this period. This expands upon the preliminary work I did in the class, writing my final essay on the political climate of Bowdoin's campus in the late 50s and early 60s. 

The corpus my group and I have created includes articles published between 1961-75 that specifically focus on the war, as well as ones covering related topics such as protests, draft resistance, and anti-war activism. The articles cover a wide range of formats, including news reports, opinion pieces, editorials, letters to the editor, interviews, and campus lectures, which, together, offer a comprehensive view of the campus by incorporating a multiplicity of parties and numerous stakeholders.

***

## Research Questions

1. How did The Bowdoin Orient's editorial language in covering the Vietnam War reflect their journalistic impartiality as a student publication, and what priorities does it reveal? *(word sentiment analysis/frequency across the entire corpus)*
2. What patterns do the types of article about Vietnam published in The Orient between 1955-75 reveal about the greater Bowdoin community during the period? *(conducting a manual content analysis by categorizing articles and analyzing them for patterns)*
3. Did The Orient's overall sentiment towards the Vietnam War change over time, and if so, how does this connect to events happening in the war? *(plotting sentiment over time - per week)*

***

## Corpus

**Reproduction:** Future DCS 2500 students have permission to use this corpus following the [CC-BY-SA-4.0 license](https://creativecommons.org/licenses/by-sa/4.0/deed.en) guidelines.

## Description

*The Bowdoin Orient* is the student-run newspaper of Bowdoin College, a private liberal arts college in Brunswick, Maine. It is one of the oldest continuously-published college newspapers in the United States, having been established in 1871. The paper is published weekly during the academic year and monthly during the summer. *The Orient* covers news, features, opinions, and arts and entertainment related to the Bowdoin College community. The paper is staffed by Bowdoin students, who are responsible for reporting, writing, editing, designing, and publishing the paper. 

**Creation Strategy:** Our group followed a relevance-driven collection methodology to acquire articles since we're matching documents to their relevance to our research questions. As a result, it was done using our search term, `Vietnam`.

### Composition

**Publication:** *The Bowdoin Orient*

**OCLC Number:** [1013419982](https://www.worldcat.org/oclc/1013419982)

**Issue Range Searched:** `v.84 - 105`

**Date Range Searched:** `01/1955 - 12/1975`

**Issue Range Actual:** `v.91 - 105`

**Date Range Actual:** `10/12/1961 - 11/14/1975`

**Search Term:** `Vietnam` (match-case not enabled)

**Size:** TBD articles (currently 133)

**Language:** `eng` (ISO 639-2 Code)

**Source:** [Bowdoin College Digital Commons](https://digitalcommons.bowdoin.edu/bowdoinorient/)

**Collection Method:** `text extraction`, `manual collection`, `crowd-sourcing`

**Workflow & Quality Assurance:** 
Bowdoin's Digital Commons makes *The Bowdoin Orient* available in PDF files each representing a volume. The publishing cycle, on average, spanned April-April. Volumes 84-105 were downloaded for this project. The 21 volumes were divided up evenly amongst the three group members so that each extracted from 7. Each volume was opened in either Adobe Acrobat where Optical Character Recognition (OCR) algorithms were used to query for the search term (`Vietnam`). Each article containing the search term was mined using a crowd-sourced manual collection of the article's text (via copy & paste into a UTF-8 encoded .txt file). No matches were returned until v.91, although v.84-90 were searched.

We are assuming that *The Orient* did not make any spelling mistakes when writing "Vietnam." Articles with these mistakes, would not have returned in our searches, and, as a result, are omitted from this corpus and subsequent analysis. 

#### Ethics Statement

The data collected for this project is derived from the publicly accessible archives of *The Bowdoin Orient*, found in the Bowdoin College Digital Commons, provided by the George J. Mitchell Department of Special Collection & Archives at the Bowdoin Library. The aim of the project is to gain a historical understanding of the attitudes and sentiments towards the Vietnam War in the Bowdoin community, as reflected in *The Orient*. The analyses will be conducted in a manner that respects the integrity of the original text and the context in which it was produced. We are aware of the potential for bias and subjectivity in the interpretation of the data, and we will strive for transparency, accuracy, and reproducability in our methodology and results. As far as possible, we will avoid making any definitive or generalized claims about the sentiments and attitudes of the Bowdoin community based solely on the data from the newspaper. Our findings will be presented in a manner that respects the diversity and complexity of views and experiences that may have existed within the community during this period.

### Methodology

#### Processing
* Removing irrelevant tags: `@TITLE=` and `@BODY=`
* Lowercasing all text.
* Removing punctuation and special characters.
* Removing stopwords - common words like "the", "and", "a", etc., that do not carry significant meaning and are therefore not useful for the analysis.
* Lemmatization - reduce words to their base form, e.g., "running" to "run", "better" to "good", etc.

<img src="images/1.png" width="750">

*Example of an article being queried for the search term. Source: pg. 35. v.91 PDF*

Each article was cross-checked for typos and punctuation errors. Due to the poor archival and digitization quality of many of the volumes, the OCR algorithms often failed to work reliably. In these cases, manual transcription of the article text was used (via typing out each word by hand). In cases where words were not clearly discernible, as shown in the example below, a best guess was applied given the context of the preceding and following sentences. We acknowledge that this is a subjective interpretation and leads to potential inaccuracy in the data, though luckily no article had its core meaning changed as a result of this.  

<img src="images/2.png" width="750">

*Example of poor archiving/digitization. Source: pg. 43, v.91 PDF*

The select terms `U.S|US`, `U.S.A|USA`, and `Viet Nam|Viet-Nam`, were re-written as `United States`, `United States of America`, and `Vietnam` respectively. Due to the physical constraints of print publication, historic newspapers such as *The Bowdoin Orient* used [abbreviations](https://web.archive.org/web/20220307224448/https://blog.newspapers.com/7-common-historical-newspaper-abbreviations-and-terms). Inconsistent terminology usage without standardization will result in measurements that are not wholly representative of the text. Furthermore, the process of removing stopwords would consider `us` and `US` as stopwords, even if they were meant as abbreviations.

#### Composition & Demarcation Assesment

**Strengths:**
* *The Bowdoin Orient* is a well-established student-run newspaper with a long history, providing a potentially unique perspective on events and issues.
* The data covers a significant time period (1955-1975) during which the Vietnam War occurred, providing a comprehensive overview of the newspaper's coverage of the conflict.

**Weaknesses:**
* The search term used (`Vietnam`) is quite broad and may result in articles that are not directly related to the Vietnam War, reducing the relevance of the data. Furthermore, it is possible that articles referred to the conflict as just that: "the conflict overseas" or just "the war." Additionally, articles covering parties directly related to the war such as Cambodia (wherein the article doesn't make an explicit reference to Vietnam) may be omitted. 
* The OCR algorithms used to extract the text from the PDF files may have resulted in errors and inaccuracies in the data not caught by the human transcribers.
* The standardization of abbreviations, while important, is subjective and may have introduced errors or inconsistencies in the data.

### Data Structure

#### File Naming Convention: `VOL_MM-DD-YYYY_TITLE.txt`

`VOL` is a three-digit integer representing the volume of the Orient that the article was found in. So, for example, volume XCVI (converted to 96) would be written as `096` in the filename.

`MM-DD-YYYY` is the date of publication of the volume the article was found in.

`TITLE` is the article title written in all caps, with periods substituting for spaces. All non-letter characters are omitted to ensure compatibility, as there is no uniform way to handle special characters in file names across operating systems. So, if the article title is published in the Orient as `"Sons and Daughters: The 'Berkeley' Bag,"` the title would be written as `"SONS.AND.DAUGHTERS.THE.BERKELEY.BAG"`

Between `VOL`, `MM-DD-YYYY`, and `TITLE`, underscores are used as delimiters.

All coming together, an article titled `"Sons and Daughters: The 'Berkeley' Bag"` published in `v.XCVI` on `April 21st, 1967` would be named `"096_04-21-1967_SONS.AND.DAUGHTERS.THE.BERKELEY.BAG"`


#### Article File Structure

Each article `.txt` file contains two pieces of useful information: `@TITLE=` and `@BODY=`

There is always a newline char `\n` between the `@TITLE=` line and the rest of the document. Using the example from before, inside the file might look like this:

`@TITLE=Sons and Daughters: The "Berkeley" Bag`

`@BODY=Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit...`

#### Directory

The collection of articles (and nothing else) is stored in `/articles`. This should be treated as a read-only folder.

***

## Analysis

### 