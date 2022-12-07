# Basic

### Data Store

Splunk stores data in index. Ingested data goes thrhough the process of indexing which converts data to sacrhcable events.

### Chaining Commands
SPL commmands use the pipe `|` commands to chain search commands together.

### [Types of commands](https://docs.splunk.com/Documentation/Splunk/9.0.2/Search/Typesofcommands)
There are six categorizations of the search commands:

* Distributable streaming
* Centralized streaming
* [Transforming](https://docs.splunk.com/Splexicon:Transformingcommand)
* Generating
* Orchestrating
* Dataset Processing


### Transforming Commands
Allow for search commands to create data structure form fields valie pairs. Frequantly used for Splink Enterprise visualizations.

### Lookup
Table mapping in Splunk for accociating key value pairs in the search output.
