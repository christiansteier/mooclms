.. _clusters:

Clusters
=========
Clusters are special group of pages in a Lesson module. A "cluster" is formed by placing a special navigational "cluster" page at the start of the group and an "end cluster" page after the last page in the group. Clusters can be considered an advanced feature of Lesson. 

What are clusters?
-------------------
The typical cluster group (or series of pages) contains question pages and we will focus our attention on this kind of cluster. It is a good practice to first add most of the content (branch table) and question pages in a lesson, then consider where to place the special navigation pages that define a cluster.

Consider a series of question pages: Q1, Q2, Q3, Q4, Q5, Q6, Q7, Q8. This represents 8 questions in a Lesson.

A cluster is started in the logical order with a cluster page. Clusters should be completed with an End of Cluster page for best results (otherwise they treat the End of Lesson as the End of Cluster).

The teacher might put some of them in a cluster, where C1 is the first "cluster" page and EC1 is the first "end cluster" page in the lesson.

    Q1, **C1**, Q2, Q3, Q4, Q5, Q6, Q7, **EC1**, Q8. 

A cluster represents a set of pages from which one or more may be randomly chosen. Questions within a cluster are randomly selected by choosing "Random Question within a Cluster" as the jump in the "Start Cluster" page. Questions within a cluster may either link to the End of Cluster to exit the cluster, or jump to any other page in the lesson. They may also jump to an unseen question within the cluster but most commonly are directed back to the "Start Cluster" page. 

Sub-Clusters
--------------
Clusters can contain sub-clusters by using Branch Tables and End of Branches. To implement this advanced feature, set up a cluster as normal with a Cluster page followed by question pages (with the jumps set up the same as above) and ended with an End of Cluster page.

    Q1, **C1**, Q2, Q3, Q4, Q5, Q6, Q7, **EC1**, Q8 

To set up a sub-cluster, wrap a group of questions with a Branch Table and an End of Branch.

    Q1, **C1**, Q2, Q3, **B1**, Q4, Q5, Q6, **EB1**, Q7, **EC1**, Q8 

Neither the content nor the jumps of the Branch Table and the End of Branch are seen by the student. Rather the two pages act as markers for the sub-cluster within the main cluster. When the student attempts the lesson, only one random question page within the sub-cluster will be displayed to the student. 

When to use a cluster?
------------------------
A cluster is used when the teacher wants a series of questions in a lesson to appear in a different random order for each student.

In the example: Q1, Q2, C1, Q3, Q4, Q5, EC1, Q6, Q7, Q8, when the student reaches C1, the teacher might set the jump to "go to an unseen question in the cluster". When a jump in Q3, Q4 and Q5 is set to go back to C1, the student will see a "new" question in the cluster. When the student has seen all the questions in the cluster, they will be sent to EC1. The student will never see EC1, just be redirected by the jump in EC1.

Any or all of the question answers inside a cluster, could exit the student from the cluster. For example, specific jumps in Q3, Q4 and Q5 could be set to Q6, thus the student would pass over EC1 and leave the cluster. 

Tips and tricks
-----------------
Remember clusters have their own adaptive logic. It is always a good idea to test a cluster when logged in as a student. New users of a cluster, might do well to create a simple lesson so they understand how clusters work when applied in a more complex adaptive lesson.

**TIP:** Setting an answer's jump to "Unseen question" may cause problems. For example, when a student has seen all the questions and is allowed to re-enter the cluster in the same lesson attempt. Clusters are an advanced feature and should be checked in a student role. 


