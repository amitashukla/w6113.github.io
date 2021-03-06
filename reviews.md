---
layout: page
---

# Paper Reviews

You are expected to write and submit a paper review of the readings before each class, and answer some questions about the readings.  The review should be akin to a conference paper review.  The purpose of the readings is to provide an illustrative example of the research area.  You are encouraged but not required to read the supplemental readings to better understand the materials.  

You can discuss questions and ask for clarifications with your colleagues and/or on piazza.  You are expected to formulate your own opinion of the reading(s) and write the review yourself.  See for a description of what we expect in paper reviews.  

We may select a random review to read and discuss in class.  This serves to highlight important characteristics of reading papers and writing good reviews.


### Submission

The first reviews ([System R](#lec2), [Postgres](#lec3)) are special, so look at the paper description for submission details.  


Otherwise, follow the following instructions: 

* [Submission form](https://goo.gl/forms/uNfVx9jUBXdj6wXd2)
* Reviews are due **10PM EST day before lecture**.  
* Late submissions are given a score of 0 without prior approval.  
* You may miss submissions for up to **2 lectures**.


### Reading Tips

Ask the following questions while readings

* What is the context of this work?
  * What was the unmet need or opportunity?  Does it make sense?
  * What were existing approaches and why do they work or not work?
  * What is the simplest example that highlights the problem that this approach works best for?
  * Does the paper (and its contributions) matter?
  * What are the actual hypotheses?
* Approach
  * How do they seek to validate their hypotheses? Do they make sense?
  * Is the evaluation cursory or deep?
  * Do you believe their results?
  * Are the results presented well?

# The Papers


<a name="lec2"/>
### System R Overview 

Readings 

* Required: <a href="./files/papers/systemr-retrospective.pdf">System R Retrospective</a>
* Optional: <a href="./files/papers/ingres-retrospective.pdf">Ingres Design</a>


Paper Review 

* System R was an impressive research and engineering effort, and the reading is a retrospective of the 6 year project.  
* The paper discusses "the Convoy Problem".  Discuss the problem:  What is it?  Why does it exist?
* The paper discusses many many topics.  Identify and pick one aspect (different than the convoy problem) that you are particularly impressed with.  Discuss what and why.
* Note: The format of this review will be different than future reviews because this is a warmup paper

Submission

* Due: 12PM Thursday 1/24 
* [SUBMIT YOUR REVIEW HERE](https://goo.gl/forms/tv0wcPqzvs3hcyNG3)


<a name='lec3' />
### INGRES/POSTGRES    

Readings

* Required: [Design of Postgres (Initial design)](./files/papers/postgres-retrospective.pdf)
* Optional: [The Postgres Next-Generation DBMS (Midterm design)](./files/papers/postgres-nextgen-cacm.pdf)
* Optional: [Design of INGRES](./files/papers/ingres-retrospective.pdf)
  * Worth skimming: QUEL, leveraging UNIX, concurrency control arguments
* Optional: [The Landsharks are on the Squawk Box - Stonebraker Turing Award Lecture](https://cacm.acm.org/magazines/2016/2/197423-the-land-sharks-are-on-the-squawk-box/fulltext)


Paper Review 

* What were the main goals for the Postgres system and why do you think they chose those goals?  Do they make sense?
* Pick one of the (many) ideas in the paper that most interests you.  Why is it interesting?   Does the proposed design hold water?  Feel free to read related work.
* Note: The format of this review will be different than future reviews because this is a warmup paper

Submission

* Due 6PM EST day before lecture
* [SUBMIT YOUR REVIEW HERE](https://goo.gl/forms/tv0wcPqzvs3hcyNG3)



<a name='lec4' />
### Column Stores    

Readings

* Required: [C-Store: A Column-oriented DBMS ](./files/papers/cstore-vldb05.pdf)
* Optional: [MonetDB/X100: Hyper-Pipelining Query Execution](./files/papers/monetdb-cidr05.pdf)
* Optional: [Integrating Compression and Execution in Column-Oriented Database Systems](./files/papers/abadi-sigmod2006.pdf)
* Optional: [An Experimental Study of Bitmap Compression vs. Inverted List Compression](./files/papers/sidm338-wangA.pdf)
* Optional: [Column-Stores vs. Row-Stores: How Different Are They Really?](http://db.csail.mit.edu/projects/cstore/abadi-sigmod08.pdf)
* Optional: [Survey: The Design and Implementation of Modern Column-Oriented Database Systems](http://db.csail.mit.edu/pubs/abadi-column-stores.pdf)
* Optional: [Blog Post: 40x faster hash joiner with vectorized execution](https://www.cockroachlabs.com/blog/vectorized-hash-joiner/)



<a name='lec5' />
### OLTP Stores    

Readings

* Required: [OLTP Through the Looking Glass, and What We Found There](./files/papers/oltpperf-sigmod08.pdf)
* Optional: [Hekaton: SQL Server’s Memory-Optimized OLTP Engine](./files/papers/hekaton-sigmod13.pdf)
* Optional: [The End of an Architectural Era](http://nms.csail.mit.edu/~stavros/pubs/hstore.pdf)



<a name='lec6' />
### Query Compilation    

Readings

* Required: [Efficiently Compiling Efficient Query Plans for Modern Hardware](./files/papers/p539-neumann.pdf)
* Optional: [How to Architect a Query Compiler, Revisited](./files/papers/tahboub-sigmod18.pdf)
* Optional: [Generating code for holistic query evaluation](./files/papers/krikellas-icde2010.pdf)
* Optional: [SMOKE: Fine-grained Lineage at Interactive Speed](./files/papers/smoke-vldb18.pdf).  An application of query compilation.
* Optional: [Spark's Scala expression compiler code](https://github.com/apache/spark/blob/master/sql/catalyst/src/main/scala/org/apache/spark/sql/catalyst/expressions/codegen/CodeGenerator.scala)

Some things to think about when reading

* For disk-based systems, when would query compilation be useful?


<a name='lec7' />
### Indexes    

Readings

* Required: [R-Trees: A Dynamic Index Structure for Spatial Searching](./files/papers/rtree-gut84.pdf)
* Optional: [Generalized Search Trees for Database Systems](./files/papers/gist-vldb95.pdf)
* Optional: [Survey: Modern B-Tree Techniques](./files/papers/btreesurvey-graefe.pdf)

Some things to think about:

* These papers extend indexes to consider multi-dimensional datasets.  Do they address the needs for modern data types (e.g., videos, images, books) and all the things we want to use this data for??  



<a name='lec8' />
### Joins   

Readings

* Required: [Shapiro: Join Processing in Database Systems with Large Main Memories](./files/papers/gracejoin-shapiro.pdf)
* Optional: [Ripple Joins for Online Aggregation](http://www.cs.cmu.edu/~natassa/courses/15-823/F02/papers/decision-ripple-sigmod99.pdf)



<a name='lec9' />
### Distributed Joins    

Readings

* Required: [Parallel Database systems: the future of high performance database systems](./files/papers/paralleldbsystems-dewitt)
* Optional: [TrackJoin](./files/papers/trackjoin-sigmod14.pdf)


<a name='lec10' />
### Exchange Operator    

Readings

* Required: [Encapsulation of parallelism in the volcano query processing system](./files/papers/volcanoparallelism-89.pdf)
* Optional: [SEDA: An Architecture for Well-Conditioned, Scalable Internet Services](http://www.sosp.org/2001/papers/welsh.pdf)

<a name='lec11' />
### Eddies  

Readings

* Required: [Eddies: Continuously Adaptive Query Processing](./files/papers/eddies-sigmod00.pdf)
* Optional: [TelegraphCQ: Continuous Dataflow Processing for an Uncertain World](http://db.csail.mit.edu/madden/html/TCQcidr03.pdf)
* Optional: [Survey: Adaptive Query Processing](https://www.nowpublishers.com/article/Details/DBS-001)



<a name='lec12' />
### Hybrid Caching/UDFs    

Readings

* Required: [Hybrid Caching](./files/papers/caching-sigmod1996.pdf)
* Optional: [Exploiting Correlations for Expensive Predicate Evaluation](https://arxiv.org/pdf/1411.3374.pdf)


<a name='lec13' />
### Top-down Optimization    

Readings

* Required: [Volcano Optimizer](./files/papers/volcanooptimizer-icde93.pdf)
* Optional: [Cascades](./files/papers/cascades-graefe.pdf)


<a name='lec14' />
### RL for Join Optimization   

Readings

* Required: [Learning to Optimize Join Queries With Deep Reinforcement Learning](https://arxiv.org/pdf/1808.03196.pdf)
* Optional: [SkinnerDB: Regret-Bounded Query Evaluation via Reinforcement Learning](https://arxiv.org/pdf/1901.05152.pdf)
* Optional: [Selectivity Estimation using Probabilistic Models](https://ai.stanford.edu/~koller/Papers/Getoor+al:SIGMOD01.pdf)


<a name='lec15' />
### Datalog and Recursion   

Readings

* Required: [Datalog and Recursive Query Processing](https://www.nowpublishers.com/article/Details/DBS-017) Chapters 2, 3
* Optional: [Evita Raced: Metacompilation for Declarative Networks](http://www.vldb.org/pvldb/1/1453978.pdf): query optimization AS datalog



<a name='lec16' />
### Lineage   

Readings:

* Required: [Provenance Semirings](http://users.ics.forth.gr/~gregkar/publications/pods2007.pdf)
* Optional: [SMOKE: Fine-grained Lineage at Interactive Speed](http://www.vldb.org/pvldb/vol11/p719-psallidas.pdf)

<a name='lec17' />
### Exploration / TBA 

Readings: TBA

<a name='lec18' />
### Fast Scans

* [BitWeaving](http://www.cs.wisc.edu/~jignesh/publ/BitWeaving.pdf)

<a name='lec19' />
### MockPC  

Readings:

* Your assigned papers


<a name='lec20' />
### MockPC  

Readings:

* Your assigned papers



<a name='lec21' />
### Materialized Views    

* Required: [Survey: Materialized Views](./files/papers/matview-survey.pdf)
* Optional: [Noria: dynamic, partially-stateful data-flow for high-performance web applications](https://pdos.csail.mit.edu/papers/noria:osdi18.pdf)


<a name='lec22' />
### Data Cubes    

* Required: [Data Cube](./files/papers/datacube-jimgray.pdf)
* Optional: [Implementing Data Cubes Efficiently](http://ilpubs.stanford.edu:8090/102/1/1995-34.pdf)
* Optional: [Explaining differences in multidimensional aggregates](./files/papers/olapdiff-sunita.pdf)

<a name='lec23' /> 
### Self-tuning DBs  

* Required: [Self-Tuning Database Systems: A Decade of Progress ](./files/papers/selftuning-chaudhuri-vldb07.pdf)
* Optional: [Automatically Indexing Millions of Databases in Microsoft Azure SQL Database](https://www.microsoft.com/en-us/research/uploads/prod/2019/02/autoindexing_azuredb.pdf)
* Optional: [Query-based Workload Forecasting for Self-Driving Database Management Systems](https://www.cs.cmu.edu/~dvanaken/papers/forecasting-sigmod18.pdf)
* Optional: [Database Cracking](https://stratos.seas.harvard.edu/files/IKM_CIDR07.pdf)


<a name='lec24' />
### Approximate Query Processing


* Required: [BlinkDB](https://sameeragarwal.github.io/blinkdb_eurosys13.pdf)
* Optional: [Pfunk-H](https://columbiaviz.github.io/files/papers/pfunk.pdf)
* Optional: [Sample+Seek](https://columbiaviz.github.io/files/papers/sigmod16sampleseek.pdf)
* Optional: [WanderJoin](https://columbiaviz.github.io/files/papers/wanderjoin.pdf)


<a name='lec25' />
### ML in DB

* Required: [MAD Skills: New Analysis Practices for Big Data](http://db.cs.berkeley.edu/papers/vldb09-madskills.pdf)
* Optional: [Towards a Unified Architecture for in-RDBMS Analytics](https://cs.stanford.edu/people/chrismre/papers/bismarck.pdf)
* Optional: [Learning Generalized Linear Models Over Normalized Data](http://pages.cs.wisc.edu/~jignesh/publ/GLMs-over-joins.pdf)
