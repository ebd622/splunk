# Manipulating Data with eval command


(14. Module 9A)
### Topics
* Understand the eval command
* Explore and perform calculations using mathematical and statistical eval functions
* Perform calculations and concatenations on field values
* Use the eval command as a function with the stats command

### Understand the eval command
TODO

### Explore and perform calculations using mathematical and statistical eval functions
[Statistical eval functions](https://docs.splunk.com/Documentation/Splunk/9.0.0/SearchReference/StatisticalFunctions):
* avg(X,...)
* max(X,...)
* min(X,...)
* random()
 
Examples
```
| makeresults | eval n = "1 3 5 6 4 2" 
| makemv n
| eval maxn = max(n)
```

[Mathematical functions](https://docs.splunk.com/Documentation/SCS/current/SearchReference/MathematicalFunctions#Mathematical_functions)
* abs(&lt;num&gt;)
* ceiling(&lt;num&gt;) or ceil(&lt;num&gt;)
* exact(&lt;expression&gt;)
* exp(&lt;num&gt;)
* floor(&lt;num&gt;)
* ln(&lt;num&gt;)
* log(&lt;num&gt;,&lt;base&gt;)
* pi()
* pow(&lt;num&gt;, &lt;exp&gt;)
* round(&lt;num&gt;, &lt;precision&gt;)
* sigfig(&lt;num&gt;)



### References
* [Eval command](https://docs.splunk.com/Documentation/SCS/current/SearchReference/EvalCommandOverview)
