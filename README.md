# Readings of Distributed System 
This git repository includes distributed system papers. It's important to read some papers for you to understand distributed system. 


## Table of Contents
* [Batch Computing](#Batch Computing)
* [Streaming Computing](#Streaming Computing)
* Distributed File System 
* Distributed Memory System 
* Key-Value System 
* Distributed Machine Learning 
* Deep Learning

## Batch Computing 
-----------------
   * [Google MapReduce](https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf)(2003 OSDI): MapReduce is a programming model and an associated implementation for processing and generating large data sets. Users specify a map function that processes a key/value pair to generate a set of intermediate key/value pairs, and a reduce function that merges all intermediate values associated with the same intermediate key<br>
      Authors: [Jeffrey Dean](https://research.google.com/pubs/jeff.html) ,  [Sanjay Ghemawa](https://research.google.com/pubs/SanjayGhemawat.html)       <br>

   * [Hadoop Online](http://www.neilconway.org/docs/nsdi2010_hop.pdf)(2010 NSDI): A modified MapReduce architecture that allows data to be pipelined between operators. This extends the MapReduce programming model beyond batch processing, and can reduce completion times and improve system utilization for batch jobs as well. It alse supports online aggregation, which allows users to see "early returns" from a job as it is being computed.<br><br>
   

## Streaming Computing
----------------------
  * [Spark Streaming](https://people.csail.mit.edu/matei/papers/2013/sosp_spark_streaming.pdf): 
