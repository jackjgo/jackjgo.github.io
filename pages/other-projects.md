---
layout: page
title: Other Projects
permalink: /other-projects
---

# Terrain
I'm broadly interested in terrain analysis algorithms and visualization.

| ![windRiver_roughness](https://raw.githubusercontent.com/jackjgo/jackjgo.github.io/gh-pages/assets/img/windRiver_roughness.JPG) |
|:--:|
| *Rougness of Wyoming's Wind River Range calculated by sd slope* |


## Vertical exaggeration
When printing 3D maps showing terrain, it's usually necessary to exaggerate elevation values. Because vertical relief is quite small relative to the scale of the earth, even large mountains appear quite flat without an exaggeration. Terrain is typically exaggerated by simply multiplying all elevation values by some factor, but different landforms require different amoounts of exaggeration to appear "right".

To alleviate this, I have a project I've called "[Dynamic Exaggeration](https://github.com/jackjgo/dynamic_exaggeration)". There are two approaches I'm following. The first is to vary exaggeration based on roughness, with rough areas (like mountains) exaggerated less than smooth areas (like open plains). This portion is done for the moment, although I do have a few ideas I want to explore, such as using a few different roughness metrics (I have only used sd slope so far).

The second approach varies exaggeration based on topographic prominence of landforms. This is still a work in progress, and has been a fun coding project. I was suprised to find that none of the usual geospatial or scientific Python packages have a prominence function.
