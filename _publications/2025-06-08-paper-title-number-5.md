---
title: "Robust Recursive Query Parallelism in Graph Database Management Systems"
collection: publications
category: conferences
permalink: /publication/robust-recursive-query-parallelism-in-gdbms
excerpt: 'This paper is about implementing runtime scheduling policies for recursive queries in GDBMSs'
date: 2025-09-04
venue: 'Proceedings of the VLDB Endowment (PVLDB), Volume 18, Issue 11'
paperurl: 'https://dl.acm.org/doi/pdf/10.14778/3749646.3749706'
---

Efficient multicore parallel processing of recursive join queries is critical for achieving good performance in graph
database management systems (GDBMSs). Prior work adopts two broad approaches. First is the state of the art morsel-driven
parallelism, whose vanilla application in GDBMSs parallelizes computations at the source node level. Second is to 
parallelize each iteration of the computation at the frontier level. We show that these approaches can be seen as part 
of a design space of morsel dispatching policies based on picking different granularities of morsels. We then empirically
study the question of which policies parallelize better in practice under a variety of datasets and query workloads that
contain one to many source nodes. We show that these two policies can be combined in a hybrid policy that issues morsels
both at the source node and frontier levels. We then show that the multi-source breadth-first search optimization from 
prior work can also be modeled as a morsel dispatching policy that packs multiple source nodes into multi-source morsels.
We implement these policies inside a single system, the Kuzu GDBMS, and evaluate them both within Kuzu and across other 
systems. We show that the hybrid policy captures the behavior of both source morsel-only and frontier morsel-only policies
in cases when these approaches parallelize well, and out-perform them on queries when they are limited, and propose it 
as a robust approach to parallelizing recursive queries. We further show that assigning multi-sources is beneficial, as 
it reduces the amount of scans, but only when there is enough sources in the query.
