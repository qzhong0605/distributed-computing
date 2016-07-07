# Readings of Distributed System 
This git repository includes distributed system papers. It's important to read some papers for you to understand distributed system. 


## <a name='toc'>Table of Contents</a>

  1. [Batch Computing](#batch-computing)
  2. [Streaming Computing](#streaming-computing)
  3. [Distributed File System](#distributed-file-system) 
  4. [Distributed Memory System](#distributed-mem-system) 
  5. [Key-Value System](#kv-system) 
  6. Distributed Machine Learning 
  7. Deep Learning

## <a name='batch-computing'>Batch Computing 
   * [MapReduce: Simplified Data Processing on Large Clusters](https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf)(2003 OSDI): This paper is a classical paper for distributed computing from Google cooperation. MapReduce is a programming model and an associated implementation for processing and generating large data sets. Users specify a map function that processes a key/value pair to generate a set of intermediate key/value pairs, and a reduce function that merges all intermediate values associated with the same intermediate key<br>
      Authors: [Jeffrey Dean](https://research.google.com/pubs/jeff.html) ,  [Sanjay Ghemawa](https://research.google.com/pubs/SanjayGhemawat.html)       <br>

   * [MapReduce Online](http://www.neilconway.org/docs/nsdi2010_hop.pdf)(2010 NSDI): A modified MapReduce architecture that allows data to be pipelined between operators. This extends the MapReduce programming model beyond batch processing, and can reduce completion times and improve system utilization for batch jobs as well. It alse supports online aggregation, which allows users to see "early returns" from a job as it is being computed.<br>
      Authors: Tyson Condie, Neil Conway, Peter Alvaro etc al.
   
   [Table of Content](#toc)

## <a name='streaming-computing'>Streaming Computing
  * [Discretized Streams: Fault-Tolerant Streaming Computation at Scale](https://people.csail.mit.edu/matei/papers/2013/sosp_spark_streaming.pdf)(2013 SOSP): A programing model. Spark Streaming is an extension of the core Spark API that enables scalable, high-throughput, fault-tolerant stream processing of the stream data.<br>
    Authors: [Matei Zaharia](https://people.csail.mit.edu/matei), [Tathagata Das](https://www.linkedin.com/in/tathadas), [Haoyuan Li](http://people.eecs.berkeley.edu/~haoyuan/), Timothy Hunter, [Scott Shenker](https://www.eecs.berkeley.edu/Faculty/Homepages/shenker.html), [Ion Stoica](http://people.eecs.berkeley.edu/~istoica/)
  * [Storm @Twitter](http://dl.acm.org/citation.cfm?id=2595641)(2014 SIGMOD): Storm is a real time fault-tolerant and distributed stream data processing system. The basic execuation unit is called topology, which includes spout and bolt. It can return result at intermidiately time, which makes it different from other distributed data processing system 

## <a name='distributed-file-system'>Distributed File System 
  * [The Google File System](https://static.googleusercontent.com/media/research.google.com/en//archive/gfs-sosp2003.pdf)(2003 SOSP): Google File System is a scalable distributed file system for data-intensive applications. It provides fault tolerance while running inexpensive commandity hardware, and it delivers aggregate performance to a lot of clients. The main differences among others <br>
    Authors: Sanjay Ghemawat, Howard Gobioff, Shun-Tak Leung

## <a name='distributed-mem-system'>Distributed Memory System
  * [Resilient Distributed Datasets: A Fault-Tolerant Abstraction for In-Memory Cluster   Computing](https://www.usenix.org/system/files/conference/nsdi12/nsdi12-final138.pdf)(2012 NSDI): Resilient Distributed DataSets, whose short name is RDD, is a distributed storage system for Spark Distributed Computing System. It's useful to execute iterative computing and cache the intermidiate result in memory. The main difference between RDD between DSM is that it's created through coarse-fined transformation. It also provides fault tolerance and scalability.  
    Authors: [Matei Zaharia](https://people.csail.mit.edu/matei), [Mosharaf Chowdhury](http://www.mosharaf.com/), [Tathagata Das](https://www.linkedin.com/in/tathadas) etc al.

## <a name='kv-system'>Key-Value System
  * [Succinct: Enabling Queries on Compressed Data](https://www.usenix.org/system/files/conference/nsdi15/nsdi15-paper-agarwal.pdf)(2015 NSDI): Succinct is a data store that enables directly queries on a compressed presentation of the input data. Succinct uses a compress technology, which is 
  archived through compressed suffix array, to make query more quickly. In addition, Succinct supports a range of queries including count and search of architary string. What differentiates Succinct from previous storage system is that it doesn't store index at all. <br>
    Authors: Rachit Agarwal, Anurag Khandelwal, [Ion Stoica](http://people.eecs.berkeley.edu/~istoica/)

