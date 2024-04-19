---
layout: page
title: "Principled Yet Practical Observability"
description: "Enhanced Trace Models for More Effective Observability in Distributed Systems"
img: assets/img/project_principled_yet_practical_observability_banner.png
importance: 1
category: work
related_publications: Huye2024
selected: true
team:
  - name: Darby Huye
    image: darby_huye.png
    role: PhD, Tufts University
  - name: Max Liu
    image: max_liu.jpeg
    role: PhD, Tufts University
  - name: Raja Sambasivan
    image: raja_sambasivan_resized.png
    role: Assistant Professor, Tufts University
  - name: Zhaoqi (Roy) Zhang
    image: zhaoqi_zhang.jpg
    role: Ph.D Student, Tufts University

---


<img style="float: right; width: 50%" src="../../assets/img/project_principled_yet_practical_observability_banner.png">

Observability in distributed systems is treated as a second-class citizen, supporting ad hoc data collection that is often unstructured and challenging to correlate across sources. Additionally, modern day observability platforms (like OpenTelemetry) use data models that prioritize ease of use for the developers but lack the expressiveness needed for complex use cases. OpenTelemtry uses the span-based model, which captures caller-callee relationships between units of execution. Research has highlighted limitations of the span-based tracing model (e.g. slack analyses) and compared this with the enhanced event-based trace model that uses happens-before relationships to capture true dependencies between events. The event-based model requires more effort from the developer along with deep knowledge of how their system works, which is not practical in an industry setting.

<!-- ![Principled Yet Practical Observability](../../assets/img/project_principled_yet_practical_observability_banner.png) -->



We argue that any enhancements made to the trace model or collection process should preserve the practicality of using the span-based trace model. To have more principled tracing data, we propose the following research directions:
- Enhance span-based traces with happens-before relationships. This will support more complex analyses including slack analysis. 
- Harness the power of ‘holes’ and hole coverings in tracing data. Currently, tracing infrastructures are plagued with data loss rendering the tracing data incomplete. These holes often go undetected since they are not explicitly marked. We are looking into ways to harness the power of these holes by downsampling data that is redundant while reducing unintentional data loss in regions that are unpredictable. 
- Change automated tools to use these enhanced data models that have holes, hole coverings, and additional happens-before relationships.

