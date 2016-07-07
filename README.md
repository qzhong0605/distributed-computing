# Readings of Distributed System 
This git repository includes distributed system papers. It's important to read some papers for you to understand distributed system. 


## <a name='toc'>Table of Contents</a>

  1. [Batch Computing](#batch-computing)
  2. [Streaming Computing](#streaming-computing)
  3. Distributed File System 
  4. Distributed Memory System 
  5. Key-Value System 
  6. Distributed Machine Learning 
  7. Deep Learning

## <a name='batch-computing'>Batch Computing 
   * [Google MapReduce](https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf)(2003 OSDI): MapReduce is a programming model and an associated implementation for processing and generating large data sets. Users specify a map function that processes a key/value pair to generate a set of intermediate key/value pairs, and a reduce function that merges all intermediate values associated with the same intermediate key<br>
      Authors: [Jeffrey Dean](https://research.google.com/pubs/jeff.html) ,  [Sanjay Ghemawa](https://research.google.com/pubs/SanjayGhemawat.html)       <br>

   * [Hadoop Online](http://www.neilconway.org/docs/nsdi2010_hop.pdf)(2010 NSDI): A modified MapReduce architecture that allows data to be pipelined between operators. This extends the MapReduce programming model beyond batch processing, and can reduce completion times and improve system utilization for batch jobs as well. It alse supports online aggregation, which allows users to see "early returns" from a job as it is being computed.<br><br>
   
   [Table of Content](#toc)

## <a name='streaming-computing'>Streaming Computing
  * [Spark Streaming](https://people.csail.mit.edu/matei/papers/2013/sosp_spark_streaming.pdf)(2013 sosp): A programing model. Spark Streaming is an extension of the core Spark API that enables scalable, high-throughput, fault-tolerant stream processing of the stream data.<br>
    Authors: [Matei Zaharia](https://people.csail.mit.edu/matei), [Tathagata Das](https://www.linkedin.com/in/tathadas), [Haoyuan Li](http://people.eecs.berkeley.edu/~haoyuan/), Timothy Hunter, [Scott Shenker](https://www.eecs.berkeley.edu/Faculty/Homepages/shenker.html), [Ion Stoica](http://people.eecs.berkeley.edu/~istoica/)
