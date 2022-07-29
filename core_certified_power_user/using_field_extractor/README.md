# Using the Field Extractor
(20. Module 12A)
(21. Module 12B)
### Topics
TODO

### Use the chart, timechart, top, rare, and stats commands to transform events into data tables
`Transforming command` is a type of search command that orders the results into a data table. 

Transforming commands "transform" the specified cell values for each event into numerical values that Splunk Enterprise can use for statistical purposes. Searches that use transforming commands are called transforming searches.

Transforming commands include `chart`, `timechart`, `stats`, `top`, `rare`, `contingency`, and `highlight`.

Transforming commands are required to transform search result data into the data structures required for visualizations such as column, bar, line, area, and pie charts.

#### `top`
Finds the most common values for the fields in the field list. Calculates **a count and a percentage** of the frequency the values occur in the events. If the <by-clause> is included, the results are grouped by the field you specify in the <by-clause>.
  
  
##### Syntax
```
top [<N>] [<top-options>...] <field-list> [<by-clause>]
```
##### Examples
```
index=web| top file  //default limit is 10
index=web| top limit=20 file
index=web| top limit=20 file showperc=false //suppress the [percent] column
```
#### `rare`
```
index=web | rare categoryId

```
#### `stats`
```
index=web | stats sum(bytes)
index=web | stats count by categoryId
```
Gives a similar result:
```
//distinct count: shows a [number]
index=web | stats dc(categoryId)

//delete duplications: shows a list with [number] hits
index=web categoryId=* | dedup categoryId
  
//shows a table with one column with [number] rows
index=web | dedup categoryId | stats list(categoryId)
```
```
index=web | stats values(referer_domain)
index=web | stats count by referer_domain, action
index=web | stats count by referer_domain, action | stats sum(count) by referer_domain
```
  
  
### References
* [Transforming command](https://docs.splunk.com/Splexicon:Transformingcommand)
