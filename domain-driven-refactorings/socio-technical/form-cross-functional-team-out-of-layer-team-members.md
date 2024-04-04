---
title: Form Cross-Functional Team out of Layer-Team Members
---

TODO: Or: Form Stream-Aligned Team out of Layer-Team Members

![](../../images/domain-driven-refactorings/socio-technical/layer-teams-to-cross-functional-team.drawio.svg)

## Motivation

When the teams in your projects are organized after technological layers, Conway’s Law (see [@Conway1968]) will inevitably bite you. Even the smallest change to your system will usually involve more than one of them. The addition of one simple field, for example, will cause work for UI team, business logic team, and database team alike. *Team Topologies* defines the idea of *fracture planes*...

When you [carve a bounded context out of the monolith](extract-bounded-context) or [build a new bounded context beside the monolith](build-new-bounded-context-from-scratch), the question arises, “which team will be responsible for the newly created bounded context?” None of the layer teams is fit for this purpose, because the new bounded context is a *vertical* and has UI, business logic, and database parts. On the other hand we can’t assign the bounded context to all the teams, because one of the rules is that it *should not belong to more than one team*.

The solution here is to form a new team that has all the required knowledge—a *cross-functional* team.

This is a typical step when the monolith splitting is accompanied or caused by what some call an *agile transition*.

## Mechanics

- Choose (at least) one person from every layer team.
- You’ll want the [early adopters]() here, not the *sceptics*. [@MannsRising201?]
- Form a new team of less than ca. nine people.
- Let the new team take responsibility for the new bounded context.
- In the new team: Encourage *t-shaping* and other agile techniques to break knowledge silos.
- For the time being let the rest of the teams organized as they are. The monolith is still there and has to be maintained.

## Example(s)
