# In Her Own Right Dataset

The In Her Own Right dataset consists of all item-level records aggregated by the project, currently 13,295.


## Metadata schema


### Table of Contents

[header - identifier](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#header---identifier)

[dc:identifier](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dcidentifier)

[Local Identifier*]

[Contributing Institution*]

[Record URL*]

[dc:title](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dctitle)

[dc:creator](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dccreator)

[dc:subject](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dcsubject)

[dc:date](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dcdate)

[dc:type](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dctype)

[dc:language](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dclanguage)

[dc:description](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dcdescription)

[dcterms:spatial*](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dctermsspatial)

[dcterms:extent](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dctermsextent)

[dc:contributor](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dccontributor)

[dc:publisher](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dcpublisher)

[dcterms:isPartOf*](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dctermsispartof)

[dc:rights](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dcrights)

[header - datestamp](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#header---datestamp)



## **header - identifier**


## **dc:identifier**

**Definition:** An unambiguous reference to the resource within a given context. 

**Repeatable:** Yes

**Required:** Yes

**Application:** Identifier must be unique within your repository.

**Example:**

    a289_001

**Mappings:**


<table>
  <tr>
   <td>Simple Dublin Core
   </td>
   <td>CONTENTDM
   </td>
   <td>MODS
   </td>
  </tr>
  <tr>
   <td>dc:identifier
   </td>
   <td>Identifier
   </td>
   <td>&lt;identifier>
   </td>
  </tr>
</table>



## **dc:title**

**Definition:** A name given to the resource.

**Repeatable:** Yes

**Required:** Yes

**Application:** InHOR will accept titles in any form. Follow DACS as much as possible. 

**Examples:**

    Letter to Hannah Darlington from Ann Preston
    Annual Meeting of the Germantown Y.W.C.A.
    Industrial Committee meeting minutes
    New Century Journal of Women's Interests, 1899

**Mappings:**


<table>
  <tr>
   <td>Simple Dublin Core
   </td>
   <td>ContentDM
   </td>
   <td>MODS
   </td>
  </tr>
  <tr>
   <td>dc:title
   </td>
   <td>Title
   </td>
   <td>&lt;titleInfo>&lt;title>
   </td>
  </tr>
</table>



## **dc:creator**

**Definition:** An entity primarily responsible for making the resource. Could be a person, family, or corporate entity.

**Repeatable:** Yes

**Required:** Yes, if known

**Application:** Before creating a local form of the creator’s name, check the following sources listed in order of preference:

* LCNAF
* VIAF
* [http://inherownright.org/](http://inherownright.org/) - another contributing repository might have already created a local form of the creator’s name.

If the creator is not found in the above sources, create a local form by following the guidelines in [Appendix A - Creating local names for “Subject” or “Creator” fields](https://docs.google.com/document/d/1RLbwdUrgIH-3YeZwhCxYSC5c4ll8q6-0_N99VwgpjEU/edit#bookmark=id.pia1rbqs3ly4)_._

**Examples:**

    Preston, Ann, 1813-1872
    Tyng, Anita Elizabeth, -1913
    Scarlett, M. J. (Mary J.)
    Woman Suffrage Society of the County of Philadelphia
    Northern Association of the City and County of Philadelphia for the Relief and Employment of Poor Women

**Mappings:**


<table>
  <tr>
   <td>Simple Dublin Core
   </td>
   <td>CONTENTDM
   </td>
   <td>MODS
   </td>
  </tr>
  <tr>
   <td>dc:creator
   </td>
   <td>Creator
   </td>
   <td>&lt;name>&lt;namePart>
   </td>
  </tr>
</table>



## **dc:subject**

**Definition:** The topic(s) of the resource.

**Repeatable:** Yes

**Required:** Yes. At least one subject is required. InHOR recommends three subjects, use more as needed.

**Application:** Typically, the subject will be represented using keywords, names, or key phrases. Generally, in considering level of description, adopt this approach: if search results brought a user to the record, would they be disappointed? InHOR recommends the following sources for subjects:

* [http://inherownright.org](http://inherownright.org) - another contributing repository might have already used a subject(s) that applies to the resource.
* FAST subject headings - a simplified version of LCSH that is easier to understand, control, apply, and use.
* Other controlled vocabularies - LCSH, AAT, LCNAF, VIAF, etc.
* Pre-selected authorized subject terms and names, compiled and recommended for use in the pilot project’s metadata enhancement event: [InHOR subject terms and names](https://docs.google.com/spreadsheets/d/1oYAhOLWHZlqjF21Ofn2a_Dx3zG50YukpqEdlt48ZJa8/edit) _(note existence of multiple tabs)_. 

If the subject is a person, family, or corporate entity and the subject is not found in the above sources, create a local form by following the guidelines in [Appendix A - Creating local names for “Creator” or "Subject" fields](https://docs.google.com/document/d/1RLbwdUrgIH-3YeZwhCxYSC5c4ll8q6-0_N99VwgpjEU/edit#bookmark=id.pia1rbqs3ly4).

For guidance on how to use LCSH, see [https://www.loc.gov/catworkshop/lcsh/](https://www.loc.gov/catworkshop/lcsh/).

**Examples**:

Names

    Elder, William
    Moseley, Nathaniel R.

Topics

    Women medical students
    Women--Education (Higher)
    Female Medical College of Pennsylvania--Students

**Mappings:**


<table>
  <tr>
   <td>Simple Dublin Core
   </td>
   <td>CONTENTDM
   </td>
   <td>MODS
   </td>
  </tr>
  <tr>
   <td>dc:subject
   </td>
   <td>Subject
   </td>
   <td>&lt;subject>
<p>
    &lt;topic>
<p>
    &lt;name>
<p>
    &lt;occupation>
<p>
    &lt;geographic>
<p>
    &lt;temporal>
<p>
    &lt;titleInfo>
   </td>
  </tr>
</table>



## **dc:date**

**Definition:** Date of creation of the physical resource.

**Repeatable:** Yes

**Required:** Yes

**Application:** Only dates formatted according to W3CDTF (ISO 8601) (YYYY-MM-DD single date or YYYY-YYYY date range) will be indexed, although anything entered in this field will be displayed. 

* If you only have an approximate date, InHOR recommends entering the date twice: once in machine-readable standard W3CDTF format (eg “1850-1860”), and a second time in a human-readable format (eg “approximately 1855”).
* If you do not have a date for the resource, instead of “undated,” use a very broad range in machine-readable W3CDTF, such as, “1850-1900”.
* For uncertain dates, because “circa” is not understood by a broad user base, the term “approximately” is preferred.

**Examples** (using the recommended ISO 8601 (W3CDTF) format YYYY-MM-DD): 

For a known date:

    1851 _OR_ 1851-01 _OR_ 1851-01-04
    
For a known date range:

    1851-03-03 - 1855-04-17 _OR_ 1851-1855
    
For an approximate date:

    1801-1855 _AND_ approximately 1851 _(note that the latter form will not be indexed by the system in its current state)_
    
For more examples see [https://www.w3.org/TR/NOTE-datetime](https://www.w3.org/TR/NOTE-datetime)  

**Mappings:**


<table>
  <tr>
   <td>Simple Dublin Core
   </td>
   <td>CONTENTDM
   </td>
   <td>MODS
   </td>
  </tr>
  <tr>
   <td>dc:date
   </td>
   <td>Date-Created
   </td>
   <td>&lt;originInfo>&lt;dateCreated>
   </td>
  </tr>
</table>



## **dc:type**

**Definition:** The nature or genre of the resource.

**Repeatable:** Yes

**Required:** Strongly recommended

**Application:** In order to map this field to InHOR, the value(s) for this element must be taken from the following list of high-level types:

* text
* image
* physical object
* sound
* moving image

This is a requirement from DPLA, which we are following to keep our data DPLA-ready. You may choose to use other values in your system, but if so, you must un-map the DC fields in the OAI export. InHOR recommends putting more specific genres (i.e. “scrapbooks” or “journals”) in the subject field. 

**Mappings:**


<table>
  <tr>
   <td>Simple Dublin Core
   </td>
   <td>CONTENTDM
   </td>
   <td>MODS
   </td>
  </tr>
  <tr>
   <td>dc:type
   </td>
   <td>Type
   </td>
   <td>&lt;typeOfResource>
   </td>
  </tr>
</table>



## **dc:language**

**Definition:** The language of the resource.

**Repeatable:** Yes

**Required:** Yes, for textual resources 

**Application:** InHOR strongly recommends that the value for this element be the 3-letter code from [ISO 639-3](https://iso639-3.sil.org/code_tables/639/data). If using [ISO 639-2](https://www.loc.gov/standards/iso639-2/php/code_list.php), given the choice between a terminology (T) code, and a bibliographic code (B), InHOR strongly recommends using the terminology code.

**Examples:**

    eng; spa; deu

**Mappings:**


<table>
  <tr>
   <td>Simple Dublin Core
   </td>
   <td>CONTENTDM
   </td>
   <td>MODS
   </td>
  </tr>
  <tr>
   <td>dc:language
   </td>
   <td>Language
   </td>
   <td>&lt;language>&lt;languageTerm>
   </td>
  </tr>
</table>



## **dc:description**

**Definition:** A free text account of the resource.

**Repeatable:** Yes

**Required:** Recommended

**Application:** Description may include but is not limited to: an abstract, a table of contents, or a free-text account of the resource.

Note that if you are contributing via OAI-PMH, transcriptions will appear on the aggregator site as a secondary “Description”. See the full text field below for further details.

**Example:**

    Copy of a letter to Hannah Darlington from Ann Preston, 1851. Hannah Darlington was a fellow Quaker from Chester County, who, like Preston, was involved in the abolition movement. In her letter to Darlington, Preston discusses her health, her enthusiasm for her studies, lectures she has attended, and mutual friends.

**Mappings:**


<table>
  <tr>
   <td>Simple Dublin Core
   </td>
   <td>CONTENTDM
   </td>
   <td>MODS
   </td>
  </tr>
  <tr>
   <td>dc:description
   </td>
   <td>Description
   </td>
   <td>&lt;abstract>
<p>
&lt;note>
<p>
&lt;table of contents>
   </td>
  </tr>
</table>



## **dcterms:spatial**

**Definition:** Spatial characteristics of the resource.

**Repeatable:** Yes

**Required:** Recommended

**Application:** Geographic location relevant to the original item. 

* InHOR requires the use of an authority list if applying geographic terms, and an applicable term can be found. Recommended, in order of preference:
    * LCNAF
    * TGN
* In addition to an authoritative term, you can add more local or granular terms/locations not in the authority list, using a locally constructed term:
    * Describe from smallest to largest unit using commas between the levels, determining the level of  granularity based on information available and the value of the detail - use any/all of the following hierarchy, retaining smallest to largest sequence
        * Street address or intersection
            * Intersection - Numbered street and cross st. e.g. 15th and Market
        * Named structure/landmark
        * Neighborhood
        * City or township
        * County
        * State/Province
        * Country, if not United States
* Always use the current street name, rather than the contemporaneous name. Use the PhillyHistory index [https://www.phillyhistory.org/historicstreets/](https://www.phillyhistory.org/historicstreets/) to historical, defunct street names for reference.

**Examples**:

Using authority list

    Philadelphia (Pa.)
    Chester (Pa. : Township)

Locally constructed term with more granularity

    Sharswood, North Philadelphia, Philadelphia, Pennsylvania
    Ben Franklin Bridge, Philadelphia, Pennsylvania

**Mappings:**


<table>
  <tr>
   <td>Simple Dublin Core
   </td>
   <td>CONTENTDM
   </td>
   <td>MODS
   </td>
  </tr>
  <tr>
   <td>dc:coverage
   </td>
   <td>Coverage-Spatial
   </td>
   <td>&lt;subject>
<p>
   &lt;geographic>
<p>
  &lt;hierarchicalGeographic>
<p>
   &lt;geographicCode>
<p>
   &lt;cartographics>
   </td>
  </tr>
</table>



## **dcterms:extent**

**Definition:** The size or duration of the resource.

**Repeatable:** Yes

**Required:** Optional

**Application:** Always include unit of measure (linear feet, pages, inches, etc.). Write out all units avoiding abbreviations, except centimeters should be written as cm (without period).** **Make sure it’s understandable for users.

**Example:**

    4 pages; 28 x 22 cm

**Mappings:**


<table>
  <tr>
   <td>Simple Dublin Core
   </td>
   <td>CONTENTDM
   </td>
   <td>MODS
   </td>
  </tr>
  <tr>
   <td>dc:format
   </td>
   <td>Format-Extent
   </td>
   <td>&lt;physicalDescription>&lt;extent>
   </td>
  </tr>
</table>



## **dc:contributor**


## **dc:publisher**

**Definition:** An entity responsible for making the original resource available (not the institution publishing the digital resource).

**Repeatable**: Yes

**Required:** Optional

**Application:** Transcribe the publisher’s name from the resource exactly as written. If no publisher is given, leave this field blank; don’t write “no publisher” or “SN.”

**Examples:**

    Philadelphia: Henry B. Ashmead Book and Job Printer
    Woman's Medical College of Pennsylvania
    Octavia Hill Association

**Mappings:**


<table>
  <tr>
   <td>Simple Dublin Core
   </td>
   <td>CONTENTDM
   </td>
   <td>MODS
   </td>
  </tr>
  <tr>
   <td>dc:publisher
   </td>
   <td>Publisher
   </td>
   <td>&lt;originInfo>&lt;publisher>
   </td>
  </tr>
</table>



## **dcterms:isPartOf**

**Definition:** Formal title of the full physical collection to which the resource belongs. If you wish to provide additional information (e.g. finding aid URL or series or box information), you may choose to use other values in your system, but if so, you must un-map the DC fields in the OAI export.

**Repeatable:** Yes

**Required:** Optional

**Application:** The database maps this field so that the user can click on a collection and see all the content from that collection that is included in the InHOR site. 

**Examples:**

    Ann Preston papers, Acc-029
    Cope Evans papers

**Mappings:**


<table>
  <tr>
   <td>Simple Dublin Core
   </td>
   <td>CONTENTDM
   </td>
   <td>MODS
   </td>
  </tr>
  <tr>
   <td>dc:source or dc:relation
   </td>
   <td>Source
   </td>
   <td>&lt;relatedItem>
   </td>
  </tr>
</table>



## **dc:rights**

**Definition:** Information about copyright or other restrictions on the use of the resource.

**Repeatable**: Yes

**Required:** Yes

**Application:** State clearly and concisely what uses are allowed and not allowed for the items in your collection. InHOR recommends selecting one of the standardized statements at [RightsStatements.org](http://rightsstatements.org/en/). Choose the statement that is most precise and permissive allowable for the materials in question. ([Creative Commons licenses](https://creativecommons.org/) are another good choice, although they are technically intended for licensing by creators, not but cultural heritage institutions.)

If your institution doesn’t have a specific practice and RightsStatements.org doesn’t suit, consider adopting the following blanket statement, using language from CLIR’s Intellectual Property (IP) Agreement. 

        Rights assessment is your responsibility. This material is made available for noncommercial educational, scholarly, and/or charitable purposes. For other uses or for more information, please contact [the repository, + contact info].

**Examples:** InHOR recommends using the following statements, listed in order of preference, as applicable.

        This work is believed to be in the Public Domain under the laws of the United States. For more information, see [http://rightsstatements.org/page/NoC-US/1.0/](http://rightsstatements.org/page/NoC-US/1.0/?language=en)
        
        This work is not in copyright, but commercial uses of this digital representation are limited. For more information, contact [the repository + contact info] and see [http://rightsstatements.org/page/NoC-NC/1.0/](http://rightsstatements.org/page/NoC-NC/1.0/)
        
        Rights assessment is your responsibility. This material is made available for noncommercial educational, scholarly, and/or charitable purposes. For other uses or for more information, please contact [the repository, + contact info].

**Mappings:**


<table>
  <tr>
   <td>Simple Dublin Core
   </td>
   <td>CONTENTDM
   </td>
   <td>MODS
   </td>
  </tr>
  <tr>
   <td>dc:rights
   </td>
   <td>Rights-License
   </td>
   <td>&lt;accessCondition>
   </td>
  </tr>
</table>



## **header - datestamp**



## **full text**
[NOT A SEPARATE FIELD - MAPS TO dc:description]

**Definition:** Transcription or OCR text.

**Repeatable:** No

**Required:** Optional

**Application:** OAI contributors: The InHOR system harvests OAI-PMH records at the object-level only. Therefore, for more complete ingest of your records, InHOR recommends placing the full document transcript at the object level -- either instead of or in addition to entering page-level transcripts. Alternatively, if you do not wish to place full document transcripts at the object level, you may submit the transcripts to InHOR via a supplemental CSV spreadsheet. If you would like to do this, contact [inhor@pacscl.org](mailto:inhor@pacscl.org) for complete instructions.

CSV contributors: The full document transcript must be entered as plain text into the single cell of the Transcription field for each object-level resource.

All contributors: Object-level transcripts will be labeled on the aggregator site as a secondary "Description".

All transcripts will be full text searchable. For transcription, InHOR recommends following the guidelines in [Appendix B](https://docs.google.com/document/d/1RLbwdUrgIH-3YeZwhCxYSC5c4ll8q6-0_N99VwgpjEU/edit#heading=h.ju9jbpcpit5c). 

## **Removed from curated tabular dataset:**
[dc:relation](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dcrelation)
[dc:coverage](https://github.com/InHerOwnRight/InHOR-Dataset/edit/main/README.md#dccoverage)

## **Acronyms and abbreviations used in these guidelines**
**AAT** - Art & Architecture Thesaurus, [http://www.getty.edu/research/tools/vocabularies/aat/](http://www.getty.edu/research/tools/vocabularies/aat/)

**CLIR** - Council on Library and Information Resources, [https://www.clir.org/](https://www.clir.org/)

**DACS** - Describing Archives: A Content Standard, [https://www2.archivists.org/standards/DACS](https://www2.archivists.org/standards/DACS)

**DC** - Dublin Core, [http://www.dublincore.org/documents/dces/](http://www.dublincore.org/documents/dces/)

**DPLA** - Digital Public Library of America, [https://dp.la/](https://dp.la/)

**FAST** - Faceted Application of Subject Terminology, [https://fast.oclc.org/searchfast/](https://fast.oclc.org/searchfast/)

**InHOR** - In Her Own Right, [http://herownright.pacscl.org/](http://herownright.pacscl.org/)

**ISO** - International Organization for Standardization, [https://www.iso.org/](https://www.iso.org/)

**LCNAF** - Library of Congress Name Authority File, [https://authorities.loc.gov/](https://authorities.loc.gov/)

**LCSH** - Library of Congress Subject Headings, [https://authorities.loc.gov/](https://authorities.loc.gov/)

**MODS** - Metadata Object Descriptive Schema, [http://www.loc.gov/standards/mods/](http://www.loc.gov/standards/mods/)

**OAI/OAI-PMH** - Open Archives Initiative-Protocol for Metadata Harvesting, [https://www.openarchives.org/pmh/](https://www.openarchives.org/pmh/)

**PACSCL** - Philadelphia Area Consortium of Special Collections Libraries, [http://pacscl.org/](http://pacscl.org/)

**RDA** - Resource Description and Access, [https://www.oclc.org/en/rda/about.html](https://www.oclc.org/en/rda/about.html)

**TGN** - Getty Thesaurus of Geographic Names, [http://www.getty.edu/research/tools/vocabularies/tgn](http://www.getty.edu/research/tools/vocabularies/tgn/index.html)

**VIAF** - Virtual International Authority File, [https://viaf.org/](https://viaf.org/)

**W3CDTF** - World Wide Web Consortium Date and Time Format, [https://www.w3.org/TR/NOTE-datetime](https://www.w3.org/TR/NOTE-datetime)


## **Parsing/record creation in InHOR application**

* How contributing institution works: code searches for the known repository names in the "rights" or "is part of" fields and parse the records based on the results. It is in either one or the other.
* Parsing: “ | “, “|”, and “;” are all interpreted by the system to indicate multiple entries in a field, and will make the entries appear as “entry1|entry2”
