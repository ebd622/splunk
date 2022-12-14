# Basic

### Data Store

Splunk stores data in index. Ingested data goes thrhough the process of indexing which converts data to sacrhcable events.

### Chaining Commands
SPL commmands use the pipe `|` commands to chain search commands together.

### [Types of commands](https://docs.splunk.com/Documentation/Splunk/9.0.2/Search/Typesofcommands)
There are six categorizations of the search commands:

* [Distributable streaming](https://docs.splunk.com/Documentation/Splunk/9.0.2/SearchReference/Commandsbytype#Streaming_commands)
* [Centralized streaming](https://docs.splunk.com/Documentation/Splunk/9.0.2/SearchReference/Commandsbytype#Streaming_commands): command applies a transformation to each event returned by a search. Unlike distributable streaming commands, a centralized streaming command only works on the search head.

* [Transforming](https://docs.splunk.com/Splexicon:Transformingcommand)
* [Generating](https://docs.splunk.com/Splexicon:Generatingcommand)
* [Orchestrating](https://docs.splunk.com/Splexicon:Orchestratingcommand)
* [Dataset Processing](https://docs.splunk.com/Documentation/Splunk/9.0.2/SearchReference/Commandsbytype#Dataset_processing)


### Transforming Commands
Allow for search commands to create data structure form fields valie pairs. Frequantly used for Splink Enterprise visualizations.

### Lookup
Table mapping in Splunk for accociating key value pairs in the search output.
