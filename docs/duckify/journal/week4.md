# Week 4

**Date:** 09.03.2026 - 13.03.2026

**Role: dev in team Tracing**

## Activities

* **Tracing pipeline implementation**
    * *Action:* Update of the palettization process
    * *Artefacts:* [Commit link](https://github.com/Toys-R-Us-Rex/Duckify/commit/029baa27dd0adeb881324274802aef5ff67be83d)

* **Plan of action documentation**
    * *Action:*  Contributions in the artefacts removals plan
    * *Artefacts:* [My plan (which was later replaced) (PDF form)](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/artefacts-removal.pdf), [The second one, made with Louis (PDF form)](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf)
---

## Blocker & resolution

* **Problem:** My 1rst attempts of the updates to remove artefacts wasn't properly documented and after reviews from my team-mate Louis, we started over.
* **Solution:** As soon as more than minor changes/updates have to be done, first lay on paper the structure of the changes to ensure a good overview of the work ahead.

* **Problem:** Some people had no job to do during days.
* **Solution:** Proactivity from the personn's part and a good overview from it's team leader and project leader.

---

## Self-reflection

> **What went well?**

- The track toward project success is maintened (but need to be overwatched)

> **What could be improved?**

- The workforce management
- My working processes

> **What did you learn?**

- Alway lay out a plan of action before implementing serious changes

---

## Hiring questions

**Q1: At some point in your team, you don't have any more work to do. How do you react ?**


**A:** I take a proactive approach. I inform the team leader whilst asking my colleagues if they would like any help.

---

**Q2: Why should you lay on paper plan of changes, then blockers/resolution before/during a important code update ?**

**A:** This process ensure that I will keep a overview of the situation as I'm working. It also serves as reference in documentation and can be easily checked/understood by my colleague. I could then ask them a review of my plan before beginning the implementation, thus recolting valuable advices. As I'm implementing the changes, it serves as a recipe to follow, ensuring that I remain on track.

---

**Q3: You've changed the palettization process. Why is your solution better now ?**

**A:** Before the changes, the palettization was made using the quantization method (MEDIANCUT),. This method is heavily biased by the
primary color in the texture, which "floods" the other colors when palettized. It's replacement with openCV KNN solution and the add of parameter to exclude a specific color from the palettization ensure that : 
    1. The main background color (in our pipeline the black, as the mask of the UV is applied on the texture before the palettization) isn't taken in account in the palette during palettization
    2. There is no more flooding of a biaised color weight. Using CNN ensure that every color as same weight.

