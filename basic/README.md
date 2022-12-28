# Basic

### Data Store

Splunk stores data in index. Ingested data goes thrhough the process of indexing which converts data to sacrhcable events.

### Chaining Commands
SPL commmands use the pipe `|` commands to chain search commands together.

### [Types of commands](https://docs.splunk.com/Documentation/Splunk/9.0.2/Search/Typesofcommands)
There are six categorizations of the search commands:

* [Distributable streaming](https://docs.splunk.com/Documentation/Splunk/9.0.2/SearchReference/Commandsbytype#Streaming_commands) command runs on the indexer or the search head, depending on where in the search the command is invoked. Distributable streaming commands can be applied to subsets of indexed data in a parallel manner.
* [Centralized streaming](https://docs.splunk.com/Documentation/Splunk/9.0.2/SearchReference/Commandsbytype#Streaming_commands): command applies a transformation to each event returned by a search. Unlike distributable streaming commands, a centralized streaming command only works on the search head.

* [Transforming](https://docs.splunk.com/Splexicon:Transformingcommand) allow for search commands to create data structure form fields valie pairs. Frequantly used for Splink Enterprise visualizations
* [Generating](https://docs.splunk.com/Documentation/Splunk/9.0.2/SearchReference/Commandsbytype#Generating_commands) fetch information from the indexes, without any transformations.
* [Orchestrating](https://docs.splunk.com/Documentation/Splunk/9.0.2/SearchReference/Commandsbytype#Orchestrating_commands) is a command that controls some aspect of how the search is processed.
* [Dataset Processing](https://docs.splunk.com/Documentation/Splunk/9.0.2/SearchReference/Commandsbytype#Dataset_processing_commands): is a command that requires the entire dataset before the command can run. Some of these commands fit into other command types in specific situations or when specific arguments are used.


### Lookup
Table mapping in Splunk for accociating key value pairs in the search output.
