---
layout: single
permalink: /W6/
title:  "Action Space in SMARTs"
categories: jekyll update
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

When designing the action space, I initially included too many possible actions, which confused the learning agent. I learned that for parking scenarios, reducing the action space to just a few discrete actions like forward, reverse, and turn is more effective.

Here’s the simplified action space I defined:

```python
actions = {
    "forward": (1.0, 0, 0),
    "reverse": (-1.0, 0, 0),
    "turn_left": (0, 0, -1.0),
    "turn_right": (0, 0, 1.0)
}
```

I also faced challenges in mapping these actions to real vehicle movements. Through trial and error, I adjusted the throttle and steering values to ensure smooth and realistic transitions. This process highlighted the importance of testing and iterating on simulations.