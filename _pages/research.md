---
layout: page
title: research
permalink: /research/
description: Vision-and-language navigation and embodied intelligence.
nav: true
nav_order: 1
---

## FlyWithMap

{: #flywithmap }

**Semantic-map-driven instruction generation for UAV vision-and-language navigation**

_Project lead · November 2025–present · Manuscript in preparation for CVPR_

UAV vision-and-language navigation often assumes that detailed navigation instructions are already available. In practical settings, a user may instead provide a high-level goal. FlyWithMap studies how to bridge this gap by generating instructions that a navigation agent can execute.

### Approach

- **Semantic environment representation.** Build building-level semantic maps from AirSim semantic segmentation, depth, and scene information.
- **Geometric planning and route abstraction.** Plan feasible 3D paths, then remove redundant waypoints according to path turns and deviations while preserving key navigation decisions.
- **Agent-adapted instruction generation.** Convert routes into natural language, controlling action order, segment organization, connection words, action vocabulary, and stopping cues.

The pipeline works with existing navigation agents **without fine-tuning them**. It lets us compare language realization strategies while holding the route, scene, and agent fixed.

### Results

Experiments across multiple navigation agents show a **9.85 percentage-point improvement in mean navigation success rate**. Different agents respond differently to how instructions are organized, motivating agent-adapted generation strategies.

This work is ongoing. The manuscript is **in preparation**.

---

## Humanoid teleoperation

{: #humanoid-teleoperation }

**Unitree H1 teleoperation data collection with Open-Teleoperation**

_Research contribution · June–August 2025_

I assisted a research group in collecting humanoid manipulation data. The setup used **Apple Vision Pro** and **Open-Teleoperation** to operate the dual arms of a **Unitree H1**, including grasping and placing target objects with multiple attributes.

My contributions included:

- Collecting continuous robot trajectories for manipulation tasks.
- Annotating action sequences with language to support vision-language-action alignment.
- Filtering motion jitter, singular poses, and semantically misaligned samples.
