# distributed-computing
This git repository is used to record my distributed computing papers. Now I'm contributing to work with distributed computing,
especailly streaming computing. I start to purchase my PhD degree at ict, cas from September in 2016. Before that, I got my 
master degree from Beihang Univeristy, where I forcused on distributed storage system.

## MapReduce<br>
   [Google MapReduce](https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf): MapReduce is a programming model and an associated implementation for processing and generating large data sets. Users specify a map function that processes a key/value pair to generate a set of intermediate key/value pairs, and a reduce function that merges all intermediate values associated with the same intermediate key<br>
   [Hadoop Online](http://www.neilconway.org/docs/nsdi2010_hop.pdf): MapReduce is a popular framework for data-intensive
   distributed computing of batch jobs. To simplify fault tolerance, many implementations of MapReduce materialize the 
   entire output of each map and reduce task before it can be consumed. In this paper, we propose a modified MapReduce architecture that allows data to be pipelined between operators. This extends the MapReduce programming model beyond batch processing, and can reduce completion times and improve system utilization for batch jobs as well. We present a modified version of the Hadoop MapReduce framework that supports online aggregation, which allows users to see “early returns”
   from a job as it is being computed. Our Hadoop Online Prototype (HOP) also supports continuous queries, which enable MapReduce programs to be written for applications such as event monitoring and stream processing. HOP retains the fault tolerance properties of Hadoop and can run unmodified user-defined MapReduce programs.
   
