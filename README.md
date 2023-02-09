# annotation_workflow_template

This repo holds the current version of the DCML annotation workflow which is pulled by all subcorpus repos upon push to their main branch. 

Please note that the `meta_ corpora` branch should be used with collections of corpora.


# Overview
|             file_name              |measures|labels|standard|                     annotators                     |reviewers|
|------------------------------------|-------:|-----:|--------|----------------------------------------------------|---------|
|wa01op05no1a_Allegretto             |      82|   120|2.3.0   |Adrian Nagel (2.1.1.), Ehsan Mohagheghi Fard (2.3.0)|AN       |
|wa01op05no1b_Tempo_di_Minuetto      |      74|   149|2.3.0   |Adrian Nagel (2.1.1), Ehsan Mohagheghi Fard (2.3.0) |AN       |
|wa02op05no2a_Allegro_di_molto       |     111|   262|2.3.0   |Adrian Nagel (2.1.1), Amelia Brey (2.3.0)           |AB, AN   |
|wa02op05no2b_Andante_di_molto       |      50|   118|2.1.1   |Adrian Nagel (2.1.1), Ehsan Mohagheghi Fard (2.3.0) |AN       |
|wa02op05no2c_Minuetto               |      28|    59|2.3.0   |Adrian Nagel (2.1.1.), Ehsan Mohagheghi Fard (2.3.0)|AN       |
|wa02op05no2d_Minore                 |      24|    39|2.3.0   |Adrian Nagel (2.1.1), Ehsan Mohagheghi Fard (2.3.0) |AN       |
|wa03op05no3a_Allegro                |      81|   191|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa03op05no3b_Allegretto             |      80|   127|2.3.0   |Adrian Nagel (2.1.1), Ehsan Mohagheghi Fard (2.3.0) |AN       |
|wa04op05no4a_Allegro                |     117|   197|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa04op05no4b_Rondeaux               |      69|   114|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa05op05no5a_Allegro_Assai          |      99|   209|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa05op05no5b_Adagio                 |      55|   130|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa05op05no5c_Prestissimo            |     102|   205|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa06op05no6a_Grave                  |      62|   148|2.3.0   |Adrian Nagel (2.1.1), Davor Krkljus (2.3.0)         |DK, AN   |
|wa06op05no6b_Allegro_Moderato       |      77|   281|2.3.0   |Adrian Nagel (2.1.1), Hanné Becker (2.3.0)          |AN       |
|wa06op05no6c_Allegretto             |      46|   155|2.3.0   |Adrian Nagel (2.1.1), Hanné Becker (2.3.0)          |         |
|wa07op17no1a_Minuetto_Con_Variatione|      18|   178|2.3.0   |Amelia Brey                                         |DK       |
|wa08op17no2a_Allegro                |     121|   186|2.3.0   |Amelia Brey                                         |DK       |
|wa08op17no2b_Andante                |      71|   144|2.3.0   |Amelia Brey                                         |DK       |
|wa08op17no2c_Prestissimo            |     101|   216|2.3.0   |Amelia Brey                                         |DK       |
|wa09op17no3a_Allegro_Assai          |     114|   268|2.3.0   |Davor Krkljus                                       |AB       |
|wa09op17no3b_Allegro                |     111|   186|2.3.0   |Davor Krkljus                                       |AB       |
|wa10op17no4a_Allegro                |      98|   226|2.3.0   |Davor Krkljus                                       |AN       |
|wa10op17no4b_Presto_Assai           |      99|   119|2.3.0   |Davor Krkljus                                       |AN       |
|wa11op17no5a_Allegro                |     102|   213|2.3.0   |Davor Krkljus                                       |ST       |
|wa11op17no5b_Presto                 |     127|   229|2.3.0   |Davor Krkljus                                       |ST       |
|wa12op17no6a_Allegro                |     118|   194|2.3.0   |Amelia Brey                                         |DK       |
|wa12op17no6b_Andante                |      74|   166|        |Amelia Brey                                         |DK       |
|wa12op17no6c_Prestissimo            |     105|   232|2.3.0   |Amelia Brey                                         |DK       |


*Overview table updated using [ms3](https://johentsch.github.io/ms3/) 1.2.2.*
