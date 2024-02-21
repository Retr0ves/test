---
layout: page
title: "Leitmotif"
description: "A novel abstraction for performance debugging of ditributed systems"
img: assets/img/12.jpg
importance: 1
category: work
related_publications: 
selected: true
team:
  - name: Mania Abdi
    image: mania_abdi.jpg
    role: PhD, Boston University
  - name: Darby Huye
    image: darby_huye.png
    role: PhD, Tufts University
  - name: Max Liu
    image: max_liu.jpeg
    role: PhD, Tufts University
  - name: Sarah Abowitz
    image: sarah_abowitz.jpeg
    role: PhD, Tufts University
  - name: Pavol Loffay
    image: pavol_loffay.jpeg
    role: Senior Software Engineer, Red Hat
  - name: Raja Sambasivan
    image: raja_sambasivan_resized.png
    role: Assistant Professor, Tufts University

---

Distributed tracing is gaining popularity and adoption, yet analyzing the end-to-end traces remains a daunting task. Traces are often large, containing hundreds of thousands of events, making them difficult to analyze and visualize.

In this work, we aim to do the heavy lifting for analying distributed traces to debug performance problems by using frequent subgraph mining to identify frequent execution patterns in distirbuted systems. With these freqeunt patterns, called workflow motifs, we can guide users to which parts of their system should be optimized to improve the overall performance.
