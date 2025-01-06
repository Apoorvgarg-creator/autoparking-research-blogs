---
layout: single
# permalink : /research-autoparking/W1/
permalink: /W1/
title:  "Learning about SMARTS"
categories: jekyll update
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

I set up SMARTS by first installing the required dependencies and cloning the SMARTS repository. Following the documentation, I set up the environment using conda. I ran into issues where some dependencies didn’t match my Python version. After some trial and error, I resolved it by creating a new environment with a specific Python version that SMARTS supports.

When I tried running the example simulation using examples/single_agent.py, I encountered a runtime error about missing SUMO binaries. I learned that installing SUMO via the recommended channel resolved the issue.

This marks the start of my journey with SMARTS and has already taught me how to troubleshoot and dig deeper into dependency conflicts.