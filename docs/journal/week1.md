# Week 1

**Date:** 16.02.2026 - 20.02.2026

**Role:** Dev in team **Tracing**

## Activities

* **General planification**
    * *Action:* Took part in the general project planification to define milestones per week. 
    * *Artefacts:* [Document file (permalink Github)](https://github.com/Toys-R-Us-Rex/Duckify/blob/1787a64b540681b7a8b219607760a1050d72c1cd/docs/planning/steps_milestones.typ)
    * *Justification:* It is necessary to have a plan of the general project evolution. This enable to anticipate difficult section to come, thus allowing to redistribute working force if needed. It also help to ensure that no unseen dependencies between teams are leftover.
    * *Skill related* communicate clearly and effectively

* **Tracing team planification**
    * *Action:* Took part in the tracing team planification to lay out a pipeline overview. 
    * *Artefacts:* [Document file (permalink Github)](https://github.com/Toys-R-Us-Rex/Duckify/blob/058f40182c9abd4c097b731ee1d95ff6e53512c0/docs/architecture/tracing/general-overview.typ)
    * *Justification:* This overview is a 1rst step in the tracing pipeline construction. This lay out a complete road to follow.
    * *Skill related* design a theoretical modelled solution

* **Research**
    * *Action:* Research a solution for texture projection solution, as this step was defined in the [General overview of the tracing process (permalink Github)](https://github.com/Toys-R-Us-Rex/Duckify/blob/058f40182c9abd4c097b731ee1d95ff6e53512c0/docs/architecture/tracing/general-overview.typ.)
    * *Artefacts:* [Research report file (permalink Github)](https://github.com/Toys-R-Us-Rex/Duckify/blob/15c1dbc08bc9060aa37bc681666f70380cd02b3d/docs/research/projection_solution.typ)
    * *Justification:* Taking time before implementation to look out for a complete solution 
    * *Result:* Promising solution found, tested but not selected.

* **Meeting report**
    * *Action:* Make a summary of a daily/weekly meeting
    * *Artefacts:*
        * [Daily meeting report file (permalink Github)](https://github.com/Toys-R-Us-Rex/Duckify/blob/be49ae5f111835d253c54c89245da1a22305db2c/docs/meetings/2026-02-19.typ)
        * [Weekly meeting report file (permalink Github)](https://github.com/Toys-R-Us-Rex/Duckify/blob/26aa4719fd0279bd80cab682a85882558017a31d/docs/meetings/weekly/2026-02-20.typ)
    * *Justification:* Need of documentation to have the overview of project evolution

## Blocker/Resolution

* **Problem:** The TEXTurePaper solution is a 2023 repo with multiple unprecised dependencies version. This made the enviromment setup error prone.
* **Solution:** First, always look in the repo issues if same problem have already been solved. If not, then find dependencies versions that work with the current system based of plausible time of implementation. Use a docker container to run the whole in closed environement.

* **Problem:** The TEXTurePaper solution used models versions not hosted anymore and specificly configured for depth.
* **Solution:** Look for alternative internet hosted models version that still exist.


## Self-Reflection
> **What went well?**

I was able to find a promising complete solution for the texture projection problem.

> **What could be improved?**

The time spent in meeting was sometimes not efficient, I could have been more proactive to insist on the productivity and the shortness of the meetings.

> **What did you learn?**

I learned :
- that I should always have existing sources of a displayed information in presentation
- that arguing about "what we will produce/not produce" is only a client's privilege
- that when testing a plausible solution, I should always push up to 5-10 cases to be able to quantify complexity


## Possible Interview Questions

**Q1: Looking for an existing solution to your problem, you find a promising one but it seems old-dated, what do you do ?**

**A:** I will use it's google scholar references to search for newer research based on the promising solution.

**Q2: Why could TEXTure have been a suitable solution for this project?**

**A:** TEXTure was a suitable solution because it is specifically designed for texture projection in 3D environments. The outputs were corresponding to our needs : a UV map of the projected texture and the texture itself in picture format. The rendering time on Calypso was in range of usage (approx. 10 min.).

**Q3: How would you approach a situation where a meeting is not led properly?**

**A:** I would take the initiative to lead the meeting. I would first reclarify the meeting's objectives and agenda, then ensure that it stays on track and that all participants have the opportunity to contribute.