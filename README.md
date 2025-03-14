![Version](https://img.shields.io/github/v/release/DCMLab/jc_bach_sonatas?display_name=tag)
[![DOI](https://zenodo.org/badge/473111841.svg)](https://doi.org/10.5281/zenodo.14996292)
![GitHub repo size](https://img.shields.io/github/repo-size/DCMLab/jc_bach_sonatas)
![License](https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-9cf)


This is a README file for a data repository originating from the [DCML corpus initiative](https://github.com/DCMLab/dcml_corpora)
and serves as welcome page for both 

* the GitHub repo [https://github.com/DCMLab/jc_bach_sonatas](https://github.com/DCMLab/jc_bach_sonatas) and the corresponding
* documentation page [https://dcmlab.github.io/jc_bach_sonatas](https://dcmlab.github.io/jc_bach_sonatas)

For information on how to obtain and use the dataset, please refer to [this documentation page](https://dcmlab.github.io/jc_bach_sonatas/introduction).

# Johann Christian Bach – Keyboard Sonatas (A corpus of annotated scores)

This corpus of annotated [MuseScore](https://musescore.org) files has been created within
the [DCML corpus initiative](https://github.com/DCMLab/dcml_corpora) and employs
the [DCML harmony annotation standard](https://github.com/DCMLab/standards).

Johann Christian, the "London Bach," pioneered an impressive number of compositional innovations
that were soon to become ubiquitous in the Classical style. In particular, he laid significant
groundwork for the development of the symphony, contributing harmonic expectations to the
new sonata-allegro form and experimenting with independent melodies in wind instruments. Though
he wrote relatively little for solo keyboard, the sonatas in this repository are no less
pivotal. Working with an early form of the pianoforte called a "Hammerflügel," Bach leveraged
the harmonic flexibility of this instrument, as well as its ability to produce subtly detailed
and balanced textures, to produce an outstanding technical exemplar for sonata composition.
It is very easy to perceive in this music the influence Bach had on his student Wolfgang Amadeus
Mozart, and indeed, three of Mozart's early concertos (those of K.107) are in fact orchestrations
of sonatas found in this repository, Bach's op. 5 nos. 2-4.

The two volumes collected in this repository are op. 5 and op. 17. The former was composed around the time of Bach's
arrival in London, prior to his appointment as music master to Queen Charlotte, while the latter appeared shortly before
Bach died indebted at 46. Both volumes demonstrate a clever combination of instrumental flash and tuneful clarity whose
influence upon the Classical style is palpable. Our annotations of these works are ideal for quantifying exactly what
those
Classical expectations are in their purest form.

## Getting the data

* download repository as a [ZIP file](https://github.com/DCMLab/jc_bach_sonatas/archive/main.zip)
* download a [Frictionless Datapackage](https://specs.frictionlessdata.io/data-package/) that includes concatenations
  of the TSV files in the four folders (`measures`, `notes`, `chords`, and `harmonies`) and a JSON descriptor:
  * [jc_bach_sonatas.zip](https://github.com/DCMLab/jc_bach_sonatas/releases/latest/download/jc_bach_sonatas.zip)
  * [jc_bach_sonatas.datapackage.json](https://github.com/DCMLab/jc_bach_sonatas/releases/latest/download/jc_bach_sonatas.datapackage.json)
* clone the repo: `git clone https://github.com/DCMLab/jc_bach_sonatas.git` 


## Data Formats

Each piece in this corpus is represented by five files with identical name prefixes, each in its own folder. 
For example, the first movement of the first sonata op. 5 no. 1 has the following files:

* `MS3/wa01op05no1a_Allegretto.mscx`: Uncompressed MuseScore 3.6.2 file including the music and annotation labels.
* `notes/wa01op05no1a_Allegretto.notes.tsv`: A table of all note heads contained in the score and their relevant features (not each of them represents an onset, some are tied together)
* `measures/wa01op05no1a_Allegretto.measures.tsv`: A table with relevant information about the measures in the score.
* `chords/wa01op05no1a_Allegretto.chords.tsv`: A table containing layer-wise unique onset positions with the musical markup (such as dynamics, articulation, lyrics, figured bass, etc.).
* `harmonies/wa01op05no1a_Allegretto.harmonies.tsv`: A table of the included harmony labels (including cadences and phrases) with their positions in the score.

Each TSV file comes with its own JSON descriptor that describes the meanings and datatypes of the columns ("fields") it contains,
follows the [Frictionless specification](https://specs.frictionlessdata.io/tabular-data-resource/),
and can be used to validate and correctly load the described file. 

### Opening Scores

After navigating to your local copy, you can open the scores in the folder `MS3` with the free and open source score
editor [MuseScore](https://musescore.org). Please note that the scores have been edited, annotated and tested with
[MuseScore 3.6.2](https://github.com/musescore/MuseScore/releases/tag/v3.6.2). 
MuseScore 4 has since been released which renders them correctly but cannot store them back in the same format.

### Opening TSV files in a spreadsheet

Tab-separated value (TSV) files are like Comma-separated value (CSV) files and can be opened with most modern text
editors. However, for correctly displaying the columns, you might want to use a spreadsheet or an addon for your
favourite text editor. When you use a spreadsheet such as Excel, it might annoy you by interpreting fractions as
dates. This can be circumvented by using `Data --> From Text/CSV` or the free alternative
[LibreOffice Calc](https://www.libreoffice.org/download/download/). Other than that, TSV data can be loaded with
every modern programming language.

### Loading TSV files in Python

Since the TSV files contain null values, lists, fractions, and numbers that are to be treated as strings, you may want
to use this code to load any TSV files related to this repository (provided you're doing it in Python). After a quick
`pip install -U ms3` (requires Python 3.10 or later) you'll be able to load any TSV like this:

```python
import ms3

labels = ms3.load_tsv("harmonies/wa01op05no1a_Allegretto.harmonies.tsv")
notes = ms3.load_tsv("notes/wa01op05no1a_Allegretto.notes.tsv")
```


## Version history

See the [GitHub releases](https://github.com/DCMLab/jc_bach_sonatas/releases).

## Questions, Suggestions, Corrections, Bug Reports

Please [create an issue](https://github.com/DCMLab/jc_bach_sonatas/issues) and/or feel free to fork and submit pull requests.

## Cite as

> Johannes Hentschel, Yannis Rammos, Markus Neuwirth, & Martin Rohrmeier. (2025). Johann Christian Bach – Keyboard Sonatas (A corpus of annotated scores) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.14996292

## License

Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License ([CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)).

![cc-by-nc-sa-image](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)

## File naming convention

```regex
wa(?<warburton>\d{2})
op(?<op>\d{2})
no(?<no>\d)
(?<movement>[a-d])_
(?<name>\S+)
```


## Overview
|             file_name              |measures|labels|standard|                     annotators                     |reviewers|
|------------------------------------|-------:|-----:|--------|----------------------------------------------------|---------|
|wa01op05no1a_Allegretto             |      82|   120|2.3.0   |Adrian Nagel (2.1.1.), Ehsan Mohagheghi Fard (2.3.0)|AN, EF   |
|wa01op05no1b_Tempo_di_Minuetto      |      74|   149|2.3.0   |Adrian Nagel (2.1.1), Ehsan Mohagheghi Fard (2.3.0) |AN, EF   |
|wa02op05no2a_Allegro_di_molto       |     111|   262|2.3.0   |Adrian Nagel (2.1.1), Amelia Brey (2.3.0)           |AB, AN   |
|wa02op05no2b_Andante_di_molto       |      50|   118|2.3.0   |Adrian Nagel (2.1.1), Ehsan Mohagheghi Fard (2.3.0) |AN, EF   |
|wa02op05no2c_Minuetto               |      28|    59|2.3.0   |Adrian Nagel (2.1.1.), Ehsan Mohagheghi Fard (2.3.0)|AN, EF   |
|wa02op05no2d_Minore                 |      24|    39|2.3.0   |Adrian Nagel (2.1.1), Ehsan Mohagheghi Fard (2.3.0) |AN, EF   |
|wa03op05no3a_Allegro                |      81|   191|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa03op05no3b_Allegretto             |      80|   127|2.3.0   |Adrian Nagel (2.1.1), Ehsan Mohagheghi Fard (2.3.0) |AN, EF   |
|wa04op05no4a_Allegro                |     117|   197|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa04op05no4b_Rondeaux               |      69|   114|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa05op05no5a_Allegro_Assai          |      99|   209|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa05op05no5b_Adagio                 |      55|   131|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa05op05no5c_Prestissimo            |     102|   205|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa06op05no6a_Grave                  |      62|   148|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa06op05no6b_Allegro_Moderato       |      77|   281|2.3.0   |Adrian Nagel (2.1.1), Hanné Becker (2.3.0)          |AN, HB   |
|wa06op05no6c_Allegretto             |      46|   155|2.3.0   |Adrian Nagel (2.1.1), Hanné Becker (2.3.0)          |AN, HB   |
|wa07op17no1a_Minuetto_Con_Variatione|      18|   178|2.3.0   |Amelia Brey                                         |DK       |
|wa08op17no2a_Allegro                |     121|   186|2.3.0   |Amelia Brey                                         |DK       |
|wa08op17no2b_Andante                |      71|   144|2.3.0   |Amelia Brey                                         |DK       |
|wa08op17no2c_Prestissimo            |     101|   216|2.3.0   |Amelia Brey                                         |DK       |
|wa09op17no3a_Allegro_Assai          |     114|   268|2.3.0   |Davor Krkljus                                       |AB       |
|wa09op17no3b_Allegro                |     111|   186|2.3.0   |Davor Krkljus                                       |AB       |
|wa10op17no4a_Allegro                |      98|   226|2.3.0   |Davor Krkljus                                       |AN       |
|wa10op17no4b_Presto_Assai           |      99|   119|2.3.0   |Davor Krkljus                                       |AN       |
|wa11op17no5a_Allegro                |     102|   214|2.3.0   |Davor Krkljus                                       |ST       |
|wa11op17no5b_Presto                 |     127|   229|2.3.0   |Davor Krkljus                                       |ST       |
|wa12op17no6a_Allegro                |     118|   194|2.3.0   |Amelia Brey                                         |DK       |
|wa12op17no6b_Andante                |      74|   166|2.3.0   |Amelia Brey                                         |DK       |
|wa12op17no6c_Prestissimo            |     105|   232|2.3.0   |Amelia Brey                                         |DK       |


*Overview table automatically updated using [ms3](https://ms3.readthedocs.io/).*
