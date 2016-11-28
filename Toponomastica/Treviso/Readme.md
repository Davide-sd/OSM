# OSM Changeset Number: 44020227
 - Link to the [changeset]
 - comment: Correzioni nella toponomastica della Citta' di Treviso
 - created_by: JOSM/1.5 (11223 en)
 - description: https://wiki.openstreetmap.org/wiki/Veneto/Numerazione_Civica
 - source: Comune di Treviso Open Data, http://dati.veneto.it/dataset/grafo-strade-toponomastica-treviso/resource/0c96817f-63cf-42c6-b219-7b540da1d5fd

## Data Set:
 - Link to the [data set]
 - Publication Date: 04/08/2016
 - License: IODL-2.0
 - Description: the data set contains all the official highway names used into the boundaries of Treviso.

## File descriptions:
 - *toponomastica-final.csv:* this file has been created by processing this [data set]. Each address was manually checked in order to correct mistypes. All the names in this file are correct!
 - *highways-treviso.csv:* by parsing all the highways found into the boundaries of Treviso (previously exported into a OSM file), the names are extracted and saved into this file. These names could be wrong: mystypes, truncation, missing parts, ...
 - *dict-high-topo.csv:* each name of highways-treviso.csv is associated to the correct name found into toponomastica-final.csv. The process is performed by a Python script implementing approximate string matching. The file has been manually checked in order to correct wrong associations.
 - *dict-addr-recheck.csv:* created by cross-checking dict-high-topo.csv's fields. It has been used to check again if the corrections were good.
 - *log-substitutions.txt:* this file contains a detailed log of all the elements that have been changed or deleted.
 - *unused-addresses.csv:* this file contains a list of correct addresses extracted from toponomastica-final.csv that are not currently mapped in Treviso.
 - *unknown-addresses.csv:* the addresses found in this list have been extracted from OSM and they are not found into toponomastica-final.csv. Some of them are addresses of adjoining cities that falls into Treviso boundaries by a few meters. The others have been created by OSM users probably to better describe what they were mapping.

  [data set]: <http://dati.veneto.it/dataset/grafo-strade-toponomastica-treviso/resource/0c96817f-63cf-42c6-b219-7b540da1d5fd>
  [changeset]: <http://www.openstreetmap.org/changeset/44020227>
