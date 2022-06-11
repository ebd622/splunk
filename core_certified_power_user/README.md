# Splunk Core Certified Power User
## Topics
* **Working with Time** ([origin](https://www.splunk.com/en_us/training/courses/working-with-time.html))
  * Searching with Time 
    * Understand the _time field and timestamps
    * View and interact with the Event Timeline
    * Use the earliest and latest time modifiers
    * Use the bin command with the _time field

  * Formatting Time
    * Use various date and time eval functions to format time

  * Comparing Index Time versus Search Time
  * Using Time Commands
    * Use the timechart command
    * Use the timewrap command

  * Working with Time Zones
    * Understand how time and timezones are represented in your data
    * Determine the time zone of your server
    * Use strftime to correct timezones in results

* **Statistical Processing** ([origin](https://www.splunk.com/en_us/training/courses/statistical-processing.html))
  * What is a Data SeriesReport Acceleration
    * Introduce data series
    * Explore the difference between single-series, multi-series, and time series data series

  * [Transforming Data](https://github.com/ebd622/splunk/tree/main/core_certified_power_user/transforming_data#transforming-data)
    * Use the chart, timechart, top, rare, and stats commands to transform events into data tables

  * Manipulating Data with eval command
    * Understand dthe eval command
    * Explore and perform calculations using mathematical and statistical eval functions
    * Perform calculations and concatenations on field values
    * Use the eval command as a function with the stats command

  * Formatting Data
    * Use the rename command
    * Use the sort command

* **Comparing Values** ([course](https://www.splunk.com/en_us/training/courses/comparing-values.html))
  * Using eval to Compare
    * Understand the eval command
    * Explain evaluation functions
    * Identify and use comparison and conditional functions
    * Use the fieldformat command to format field values

  * Filtering with where
    * Use the where command to filter results
    * Use wildcards with the where command
    * Filter fields with the information functions, isnull and isnotnull

* **Result Modification** ([course](https://www.splunk.com/en_us/training/courses/result-modification.html))
  * Manipulating Output
    * Convert a 2-D table into a flat table with the untable command
    * Convert a flat table into a 2-D table with the xyseries command

  * Modifying Result Sets
    * Append data to search results with the appendpipe command
    * Calculate event statistics with the eventstats command
    * Calculate "streaming" statistics with the streamstats command
    * Modify values to segregate events with the bin command

  * Managing Missing Data
    * Find missing and null values with the fillnull command

  * Modifying Field Values
    * Understand the eval command
    * Use conversion and text eval functions to modify field values
    * Reformat fields with the foreach command

  * Normalizing with eval
    * Normalize data with eval functions
    * Identify eval functions to use for data and field normalization

* Correlation Analysis ([course](https://www.splunk.com/en_us/training/courses/correlation-analysis.html))
  * [Calculate Co-Occurrence Between Fields](https://github.com/ebd622/splunk/blob/main/core_certified_power_user/calculate-between-fields/README.md#calculate-co-occurrence-between-fields)
    * Understand transactions
    * Explore the transaction command

  * Analyze Multiple Datasets
    * Understand subsearch
    * Use the append, appendcols, union, and join commands to combine, analyze, and compare multiple data sources


* Creating Knowledge Objects ([course](https://www.splunk.com/en_us/training/courses/creating-knowledge-objects.html))
  * Knowledge Objects and Search-time Operations
    * Understand role of knowledge objects for enriching data
    * Define search-time operation sequence
  * Creating Event Types
    * Define event types
    * Create event types using three methods
    * Tag event types
    * Compare event types and reports

  * Using Event Type Builder
  * Creating Workflow Actions
  * Creating Tags and Aliases
  * Creating Search Macros

* Creating Field Extractions ([course](https://www.splunk.com/en_us/training/courses/creating-field-extractions.html))
  * Using the Field Extractor
    * Understand types of extracted fields and when they are extracted
    * Explore the Splunk Web Field Extractor (FX)

  * Creating Regex Field Extractions
    * Identify basics of regular expressions (regex)
    * Understand the regex field extraction workflow
    * Edit regex for field extractions

  * Creating Delimited Field Extractions
    * Identify delimited field values in event data
    * Understand the delimited field extraction workflow


* Data Models ([course](https://www.splunk.com/en_us/training/courses/data-models.html))
