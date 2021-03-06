# Readings of Distributed System 
This git repository includes distributed system papers. It's important to read some papers for you to understand distributed system. 


## <a name='toc'>Table of Contents</a>

  1. [Batch Computing](#batch-computing)
  2. [Streaming Computing](#streaming-computing)
  3. [Distributed File System](#distributed-file-system) 
  4. [Distributed Memory System](#distributed-mem-system) 
  5. [Key-Value System](#kv-system) 
  6. [Resource Sharing and Scheduling System](#rs-sharing-scheduling)
  7. Distributed Machine Learning 
  8. Deep Learning
  9. [Other Resources](#other-resources)

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
  
  [Table of Contents](#toc)

## <a name='distributed-file-system'>Distributed File System 
  * [The Google File System](https://static.googleusercontent.com/media/research.google.com/en//archive/gfs-sosp2003.pdf)(2003 SOSP): Google File System is a scalable distributed file system for data-intensive applications. It provides fault tolerance while running inexpensive commandity hardware, and it delivers aggregate performance to a lot of clients. The main differences among others <br>
    Authors: Sanjay Ghemawat, Howard Gobioff, Shun-Tak Leung

  [Table of Contents](#toc)

## <a name='distributed-mem-system'>Distributed Memory System
  * [Resilient Distributed Datasets: A Fault-Tolerant Abstraction for In-Memory Cluster   Computing](https://www.usenix.org/system/files/conference/nsdi12/nsdi12-final138.pdf)(2012 NSDI): Resilient Distributed DataSets, whose short name is RDD, is a distributed storage system for Spark Distributed Computing System. It's useful to execute iterative computing and cache the intermidiate result in memory. The main difference between RDD between DSM is that it's created through coarse-fined transformation. It also provides fault tolerance and scalability.  
    Authors: [Matei Zaharia](https://people.csail.mit.edu/matei), [Mosharaf Chowdhury](http://www.mosharaf.com/), [Tathagata Das](https://www.linkedin.com/in/tathadas) etc al.
  
  [Table of Contents](#toc)

## <a name='kv-system'>Key-Value System
  * [Succinct: Enabling Queries on Compressed Data](https://www.usenix.org/system/files/conference/nsdi15/nsdi15-paper-agarwal.pdf)(2015 NSDI): Succinct is a data store that enables directly queries on a compressed presentation of the input data. Succinct uses a compress technology, which is 
  archived through compressed suffix array, to make query more quickly. In addition, Succinct supports a range of queries including count and search of architary string. What differentiates Succinct from previous storage system is that it doesn't store index at all. <br>
    Authors: Rachit Agarwal, Anurag Khandelwal, [Ion Stoica](http://people.eecs.berkeley.edu/~istoica/)
  * [Bigtable: A Distributed Storage System for Structured Data](https://static.googleusercontent.com/media/research.google.com/en//archive/bigtable-osdi06.pdf)(2006 OSDI): Bigtable is a distributed storage system for managing structured data to scale to a very large size: Petabytes of data across thousands of commondity servers. A Bigtable is a sparse, distributed, persistent multi-dimensional sorted map. This map is indexed by row key, column key and timestamp key. The value is an uninterpreted array of bytes. It's a single-master distributed storage system. The underlying data structure for data storage is Log-Structued Merge Tree.  
  
  [Table of Contents](#toc)

## <a name='rs-sharing-scheduling'>Resource Sharing System
  * [Mesos: A Platform for Fine-Grained Resource Sharing in the Data Center](http://dl.acm.org/citation.cfm?id=1972488)(2011 NSDI): Mesos is a platform for sharing commondity clusters between multiple diverse cluster computing frameworks, such as Hadoop and MPI. Sharing improves cluster utilization and avoid per-framework data replication. Mesos shares resouces in fined-grained manner, allowing frameworks to achieve data locality by take turns reading data stored on each machine.
  
  [Table of Contents](#toc)

## <a name='other-resources'> Other Resources
  * [Operating Systems Reading Group](https://www.cl.cam.ac.uk/~ms705/netos/os-reading-group.html): Here is Operating Systems reading group from University of Cambrige. There are many interesting and fantastic papers in here, including traditional operation system and trends on operation system, such as libraos, plan9 etc al. You can choose what you are interested in to dive into it.
  * [Readings in Databases](https://github.com/rxin/db-readings): A list of papers essential to understanding databases and building new data processing systems.   
  * [Stream Processing Papers](https://cwiki.apache.org/confluence/display/SAMZA/Stream+Processing+Papers): Here includes stream processing and stream algorithm. You can find many interesting papers focused on streaming processing.
  
  [Table of Contents](#toc)
