---
layout: single
permalink: /W4/
title:  "Q-Learning"
categories: jekyll update
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

Defining the states and actions for the parking scenario was more complex than I anticipated. Initially, my state representation was too granular, which led to a massive Q-table that was difficult to manage. I simplified it by grouping parking spaces into broader zones.

Here’s how I initialized my Q-table:

```python
q_table = defaultdict(lambda: [0] * num_actions)
```

Another obstacle was the reward function. The agent initially got stuck in loops where it kept making unproductive moves. I resolved this by introducing a small negative reward for every step to encourage efficiency. Debugging these issues taught me to iterate on both code and logic incrementally.
