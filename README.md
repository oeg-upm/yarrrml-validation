# Validation fo Human-friendly mapping serializations


This repository contains the test cases for YARRRML, and their corresponding translation (when it is possible) to XRM, SMS2, and ShExML.


## System support


* YARRRRML: [YATTER](https://github.com/oeg-upm/yatter) and [YARRRML-parser](https://github.com/RMLio/yarrrml-parser)
* SheXML: [ShExML  translator](https://github.com/herminiogg/ShExML)
* SMS: [Stardog (supporting R2RML)](https://www.stardog.com/)
* XRM: [XRM Translator](https://zazuko.com/products/expressive-rdf-mapper/)

|Features                        |YATTER|YARRRML parser|ShExML  translator|Stardog (to RDF)|XRM  Translator|
|:------------------------------:|:----------------:|:------------:|:----------------:|:--------------:|:-------------:|
|          [R2]RML-core          |      23/23       |    18/23     |     18/18**      |     13/13      |     11/11     |
|            RML-star            |       6/6        |     N/A      |       N/A        |      2/2       |      N/A      |
|          RML-language          |       3/3        |     3/3      |       3/3        |      3/3       |      1/1      |
|          RML-datatype          |       2/2        |     N/A      |       0/2        |      N/A       |      N/A      |
|           RML-target           |       6/6        |     6/6      |       N/A        |      N/A       |      N/A      |
|         RML-functions          |      10/10       |    0/10*     |       0/4        |      6/6       |      N/A      |
| Total w.r.t. its serialization |   100% (50/50)   | 64% (27/42)  |   77% (21/27)    |  100% (24/24)  | 100% (12/12)  |
|   Total w.r.t. all features    |   100% (50/50)   | 54% (27/50)  |   42% (21/50)    |  48% (24/50)   |  24% (12/50)  |


\* It supports functions but translates to another specification

\*\* Only online sources are supported, local ones are not correctly translated to RML 
