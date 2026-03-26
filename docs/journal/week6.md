# Week 6

**Date:** 23.03.2026 - 27.03.2026

**Role: dev in team Tracing**

## Activities

* **Update the UV map disposition**
    * *Action:* Remapping the UV using the same duck model, to ensure that all UV blocks are away from each others.
    * *Artefacts:* [PR link](https://github.com/Toys-R-Us-Rex/Duckify/pull/90)

* **Reduce points amount per traces**
    * *Action:* Based on comments from the robot team, objective was to reduce the amount of traces, thus to reduce the amount of points in contours.
    * *Artefacts:* [PR link](https://github.com/Toys-R-Us-Rex/Duckify/pull/92)

* **Fill slicing debugging 2**
    * *Action:* Solve bug found after the reduction update
    * *Artefacts:* [PR link](https://github.com/Toys-R-Us-Rex/Duckify/pull/96)

* **Create new tests and masks**
    * *Action:* From a demand by the team robot, create new motives in Blender then Traces files for tests with the robot, with new masks to only cover precise zone
    * *Artefacts:* [PR link](https://github.com/Toys-R-Us-Rex/Duckify/pull/99)

* **Tracing pipeline stress-test**
    * *Action:* During the project, the tracing pipeline had multiples updates and debug phases since it's first implementation. At this point, the pipeline is for sure effective when used with the textures tested during our implementation work. To further tests and discover possible flaws, it should be further tested with new textures.
    * *Artefacts:* 

## Blocker & resolution

* **Problem:** Solving the reduction theme, it created new problems. I should have anticipated them, at least tried to.
* **Solution:** Taking a step back on the solution implemented and trying to find possible impacts on the rest of the pipeline.

---

## Self-reflection

> **What went well?**

- The resolution of te points amount per traces when smoothly. The good previous pipline implementation, with parametrization of changing variable proved to be a good ground working field.

> **What could be improved?**

- When working for a demand from another group, always make sure to cleary understand (me and them) the goal to reach and try too questions limits and evolution scope. This to reduce further double work if changes appear.

> **What did you learn?**

- When process updates (for example the UV map or the team robot advances), redoing work can be obligatory.

---

## Hiring questions

**Q1: There has been a late addition of toggles of the differents debug visualisations added this week, isn't it late ?**


**A:** It should indeed have been done cleary earlier. Getting all the visualitions when working/debugging wasn't overloading until this week. This explain why this change hasn't been done before. It's not the only one of it's kind. We (the tracing team) have, having in mind that it's a prototype, always prioritise working on effectiveness toward the final goal over quality of life implementations.

---

**Q2: ?**

**A:** 

---

**Q3: ?**

**A:**


