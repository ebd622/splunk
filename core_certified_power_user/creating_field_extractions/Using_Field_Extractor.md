# Using the Field Extractor
(20. Module 12A)
(21. Module 12B)
### Topics
* Understand types of extracted fields and when they are extracted
* Explore the Splunk Web Field Extractor (FX)


#### Understand types of extracted fields and when they are extracted
Field extraction methods:
* Regex: used for Unstructured data
* Delimiters: used for Structured data
* Commands: work with `rex` and `erex` in your SPL
    * `rex` - use `regex` to create a new fields our of a feild that already exists (when you a `regex` pro). This is a key-point with `rex`;
    * `erex` - aids (helps) in generating regex for field extraction as long as you provide exanples of what you want to extract.

#### Explore the Splunk Web Field Extractor (FX)
There are a few ways to nvigate to Web Field Extractor:
* Settings -> Fields -> Fields Extractions -> Open Field Extractor;
* Jump to it from your events action drop down menu;
* Go to the buttom on the fields menu and click `Extract new fields`


  
### References
* [rex)](https://docs.splunk.com/Documentation/SplunkCloud/8.2.2203/SearchReference/Rex)

