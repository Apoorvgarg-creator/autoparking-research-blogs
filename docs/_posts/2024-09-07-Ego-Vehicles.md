---
layout: single
permalink: /W2/
title:  "Learning about Ego Vehicles"
categories: jekyll update
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

Understanding the ego vehicle’s role was straightforward, but customizing its position in the map.net.xml file posed challenges. The XML structure was complex, with multiple edge and lane elements. Initially, I didn’t know which coordinates corresponded to specific map locations. I resolved this by visualizing the map using a SUMO GUI tool, which helped me locate nodes and lanes visually.

Here’s an example of how I modified an edge in the XML:

```xml
<edge id="edge-1" from="node-3" to="node-4" numLanes="3">
  <lane index="2" length="50" shape="..."/>
</edge>
```
After updating the file, I ran the simulation and observed that the ego vehicle started at the desired position. Learning to use visualization tools saved me from trial-and-error editing of XML files.


