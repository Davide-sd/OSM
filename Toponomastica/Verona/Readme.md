# OSM Changeset Number: 44165602
 - Link to the [changeset]
 - comment: Correzioni nella toponomastica della Citta' di Verona
 - created_by: JOSM/1.5 (11223 en)
 - description: https://wiki.openstreetmap.org/wiki/Veneto/Numerazione_Civica
 - source: Comune di Verona Open Data, License IODL-2.0, Stradario (http://www.comune.verona.it/nqcontent.cfm?a_id=37264)

## Data Set:
 - Link to the [data set]
 - Publication Date: 29/11/2016
 - License: IODL-2.0
 - Description: the data set contains all the official highway names used into the boundaries of Vicenza.

## File descriptions:
 - *toponomastica-final.csv:* this file has been created by processing this [data set]. Each address was manually checked in order to correct mistypes. All the names in this file are correct!
 - *highways-verona.csv:* by parsing all the highways found into the boundaries of Verona (previously exported into a OSM file), the names are extracted and saved into this file. These names could be wrong: mystypes, truncation, missing parts, ...
 - *dict-high-topo.csv:* each name of highways-verona.csv is associated to the correct name found into toponomastica-final.csv. The process is performed by a Python script implementing approximate string matching. The file has been manually checked in order to correct wrong associations.
 - *highways-verona-new.csv:* created by the same script as highways-verona.csv. Analyzing and correcting the associations found into dict-high-topo.csv could take several days. In the mean time, new highways could be added or changes to the existing ones could be made. We need to extract the updated data from OSM.
 - *new-addresses.csv:* this file has been created by intersection of highways-verona.csv and highways-verona-new.csv. It contains a list of new addresses that we need to take into account in the dict-high-topo.csv.
 - *log-substitutions.txt:* this file contains a detailed log of all the elements that have been changed or deleted.
 - *unused-addresses.csv:* this file contains a list of correct addresses extracted from toponomastica-final.csv that are not currently mapped in Verona.
 - *unknown-addresses.csv:* the addresses found in this list have been extracted from OSM and they are not found into toponomastica-final.csv. Some of them are addresses of adjoining cities that falls into Verona boundaries by a few meters. The others have been created by OSM users probably to better describe what they were mapping.

  [data set]: <https://www.comune.verona.it/nqcontent.cfm?a_id=38807>
  [changeset]: <http://www.openstreetmap.org/changeset/44165602>
