---
layout: page
title: reach out
permalink: /reach-out

nav: true
nav_order: 8
---

#### Jiayi Dong and Anshul Rastogi, Locating regions of uncertainty in distributed systems using aggregate trace data (15 Jan 2023)

Distributed systems are central to countless applications in the modern world. These applications can have tens to thousands of components interacting making it difficult to identify the source of performance problems. Distributed tracing is widely used to elucidate the interactions within a distributed system; however, instrumenting system codebases can be tedious, and collecting tracing data generates overhead. Optimally, minimal instrumentation is added to regions of the codebase that explains the majority of the system's performance variation. We present a prototype application that highlights regions of performance uncertainty in a system, guiding developers to where instrumentation would most increase predictability. Using aggregate trace data, spans are ranked by uncertainty metrics, which are primarily the standard deviation and coefficient of variation of the exclusive latencies of an operation across multiple traces. We developed our prototype in Python and applied it to trace data extracted from HotROD. We evaluated our tool on four test scenarios where we injected latency into services in HotROD. Our tool highlights the service(s) with injected latency in all four test cases.


####  Tanmay Gupta and Anshul Rastogi, Threshold-Based Inference of Dependencies in Distributed Systems (31 Dec 2021)

Many current online services rely on the interaction between different components that form a distributed system. Analyzing distributed systems is important in performance analysis (e.g. critical path analysis), debugging, and testing newfeatures. However, the analysis of these systems can be difficult due to limited knowledge of how components work and the variety of services and applications that are usually instrumented. The Mystery Machine , introduced by Chow et al. in 2014, has a “big data” approach, using logged events across many traces to generate and refine a causal model. We introduce Scooby Systems , our extension of The Mystery Machine ’s algorithm. We introduce thresholds to increase the tolerance to violations in the formation of causal relationships. In the future, we hope to improve Scooby Systems ’s scalability with a Hadoop MapReduce implementation.


#### Neel Bhalla, Constructing Workflow-centric Traces in Close to Real Time for the Hadoop File System (22 Jul 2020)

Diagnosing problems in large scale systems using cloud based distributed services is a challenging problem. Workflow-centric tracing captures the workflow (work done to process requests) and dependency graph of causally-related events among the components of a distributed system. But, constructing traces has historically been performed offline in batch fashion, so trace data is not immediately available to engineers for their diagnosis efforts. In this work, we present an approach based on graph abstraction and streaming framework to construct workflow-centric traces in near real time for the Hadoop file system. This approach will provide the network operators with a real time understanding of the distributed system behavior.


#### Harshal Sheth, Nihar Sheth, and Aashish Welling, Read-Copy Update in a Garbage Collected Environment (1 Mar 2017)

Read-copy update (RCU) is a synchronization mechanism that allows efficient parallelism when there are a high number of readers compared to writers. The primary use of RCU is in Linux, a highly popular operating system kernel. The Linux kernel is written in C, a language that is not garbage collected, and yet the functionality that RCU provides is effectively that of a “poor man’s garbage collector” (P. E. McKenney). RCU in C is also complicated to use, and this can lead to bugs. The purpose of this paper is to investigate whether RCU implemented in a garbage collected language (Go) is easier to use while delivering comparable performance to RCU in C. This is tested through the implementation and benchmarking of 4 linked lists, 2 using RCU and 2 using mutexes. One RCU linked list and one mutex linked list are implemented in each language. This paper finds that RCU in a garbage collected language is indeed significantly easier to use, has similar overall performance to, and on very high read loads, outperforms, RCU in C.


<div class="publications">

{% bibliography -f mit_prime_papers.bib %}

</div>

