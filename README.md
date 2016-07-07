# Readings of Distributed System 
This git repository includes distributed system papers. It's important to read some papers for you to understand distributed system. 


## Table of Contents
* batch computing 
* streaming computing 
* distributed file system 
* distributed memory system 
* key-value system 
* document-oriented system 

## Batch Computing <br>
   * [Google MapReduce](https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf)(2013 OSDI) MapReduce is a programming model and an associated implementation for processing and generating large data sets. Users specify a map function that processes a key/value pair to generate a set of intermediate key/value pairs, and a reduce function that merges all intermediate values associated with the same intermediate key<br><br>
   * [Hadoop Online](http://www.neilconway.org/docs/nsdi2010_hop.pdf)(2010 NSDI) A modified MapReduce architecture that allows data to be pipelined between operators. This extends the MapReduce programming model beyond batch processing, and can reduce completion times and improve system utilization for batch jobs as well. It alse supports online aggregation, which allows users to see "early returns" from a job as it is being computed.<br><br>
   
   
