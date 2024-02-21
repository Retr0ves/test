---
layout: page
title: Pythia
description: "VAIF: Variance-driven Automated Instrumentation Framework for diagnosing performance problems in distributed applications"
img: assets/img/12.jpg
importance: 1
category: work
related_publications: Toslali2021, Ates:2019th
selected: true
team:
  - name: Emre Ates
    image: emre_ates_cropped.png
    role: PhD, 2020, Boston University
  - name: Mert Toslali
    image: mert_toslali_resized.png
    role: PhD, Boston University
  - name: Lily Sturmann
    image: lily_sturmann_resized.png
    role: Software Engineer, Red Hat
  - name: Pavol Loffay
    image: pavol_loffay.jpeg
    role: Senior Software Engineer, Red Hat
  - name: Ayse Coskun
    image: ayse_coskun_resized.png
    role: Professor, Boston University
  - name: Raja Sambasivan
    image: raja_sambasivan_resized.png
    role: Assistant Professor, Tufts University

---

Developers use logs to diagnose performance problems in distributed applications. However, it is difficult to know a priori where logs are needed and what information in them is needed to help diagnose problems that may occur in the future. 

We present the Variance-driven Automated Instrumentation Framework (VAIF), which runs alongside distributed applications. In response to newly-observed performance problems, VAIF automatically searches the space of possible instrumentation choices to enable the logs needed to help diagnose them. 

To work, VAIF combines distributed tracing (an enhanced form of logging) with insights about how response-time variance can be decomposed on the critical-path portions of requests’ traces. We evaluate VAIF by using it to localize performance problems in OpenStack and HDFS. We show that VAIF can localize problems related to slow code paths, resource contention, and problematic third-party code while enabling only 3-34% of the total tracing instrumentation.
