![Version](https://img.shields.io/github/v/release/DCMLab/jc_bach_sonatas?display_name=tag)
[![DOI](https://zenodo.org/badge/{{ zenodo_badge_id }}.svg)](https://zenodo.org/badge/latestdoi/{{ zenodo_badge_id }})
![GitHub repo size](https://img.shields.io/github/repo-size/DCMLab/jc_bach_sonatas)
![License](https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-9cf)


This is a README file for a data repository originating from the [DCML corpus initiative](https://github.com/DCMLab/dcml_corpora)
and serves as welcome page for both 

* the GitHub repo [https://github.com/DCMLab/jc_bach_sonatas](https://github.com/DCMLab/jc_bach_sonatas) and the corresponding
* documentation page [https://dcmlab.github.io/jc_bach_sonatas](https://dcmlab.github.io/jc_bach_sonatas)

For information on how to obtain and use the dataset, please refer to [this documentation page](https://dcmlab.github.io/jc_bach_sonatas/introduction).

# Johann Christian Bach – Keyboard Sonatas
This corpus of annotated [MuseScore](https://musescore.org) files has been created within
the [DCML corpus initiative](https://github.com/DCMLab/dcml_corpora) and employs
the [DCML harmony annotation standard](https://github.com/DCMLab/standards).

Johann Christian, the "London Bach," pioneered an impressive number of compositional innovations\r
that were soon to become ubiquitous in the Classical style. In particular, he laid significant\r
groundwork for the development of the symphony, contributing harmonic expectations to the\r
new sonata-allegro form and experimenting with independent melodies in wind instruments. Though\r
he wrote relatively little for solo keyboard, the sonatas in this repository are no less\r 
pivotal. Working with an early form of the pianoforte called a "Hammerflügel," Bach leveraged\r
the harmonic flexibility of this instrument, as well as its ability to produce subtly detailed\r
and balanced textures, to produce an outstanding technical exemplar for sonata composition.\r
It is very easy to perceive in this music the influence Bach had on his student Wolfgang Amadeus\r
Mozart, and indeed, three of Mozart's early concertos (those of K.107) are in fact orchestrations\r
of sonatas found in this repository, Bach's op. 5 nos. 2-4.

The two volumes collected in this repository are op. 5 and op. 17. The former was composed around\r the time of Bach's arrival in London, prior to his appointment as music master to Queen Charlotte,\r while the latter appeared shortly before Bach died indebted at 46. Both volumes demonstrate a\r clever combination of instrumental flash and tuneful clarity whose influence upon the Classical\r style is palpable. Our annotations of these works are ideal for quantifying exactly what those\r
Classical expectations are in their purest form.

## Cite as

## Version history

See the [GitHub releases](https://github.com/DCMLab/jc_bach_sonatas/releases).

## Questions, Suggestions, Corrections, Bug Reports

Please [create an issue](https://github.com/DCMLab/jc_bach_sonatas/issues) and/or feel free to fork and submit pull requests.

## License

Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License ([CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)).

![cc-by-nc-sa-image](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)

## File naming convention

```regex
wa(?<warburton>\d{2})
op(?<op>\d{2})
no(?<no>\d)
(?<movement>a|b|c|d)_
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
