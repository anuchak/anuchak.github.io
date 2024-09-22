---
permalink: /
title: "About"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi ! Welcome to my page.   
I'm a 1st year PhD student at the [David R. Cheriton School of Computer Science, University of Waterloo](https://cs.uwaterloo.ca/). I'm part of the [Data Systems Group (DSG) Lab](https://uwaterloo.ca/data-systems-group/), advised by Prof. [Semih Salihoğlu](https://cs.uwaterloo.ca/~ssalihog/).  

I recently completed my Master’s Thesis (MMath CS), also from the University of Waterloo.
Prior to this, I worked as a Software Engineer for 2 years at Goldman Sachs.

## Research Interests

- Databases
- Graph Data Management

I'm currently involved with [Kùzu](https://github.com/kuzudb/kuzu) a new graph database (GDBMS) for analytical workloads.
Kùzu is a single node disk-based columnar GDBMS with support for processing larger than memory datasets, a vectorized query
execution engine and MVCC for transactions. 

For my [Master's Thesis](https://uwspace.uwaterloo.ca/items/0476a252-457c-4633-bac5-b7f2e7fb3727) I worked on efficient scheduling policies for
handling recursive joins in Kùzu. I modified Kùzu's default morsel-driven scheduling policy to parallelize a single recursive computation (frontier-based parallelism) while
also executing multiple concurrent recursive computations (vanilla morsel-driven parallelism) to gain query speedups.

In general, I am interested in database internals and enjoy low-level systems programming (primarily C++).

Contact: a8chakra [at] uwaterloo [dot] ca
