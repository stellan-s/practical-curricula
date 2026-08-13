# Practical Systems Thinking

> This curriculum was developed with AI assistance and has not been independently validated.

**Goal:** Learn to see structure behind events, model feedback and accumulation, identify leverage, and apply the method to real problems.

**Total:** Approximately 10–12 hours.

**Rule:** Use one real system throughout the course. Do not merely take notes.

## 1. Stop thinking in parts — 45 min

**Watch**

- [Systems Thinking: A Little Film About a Big Idea — Cabrera Lab](https://www.youtube.com/watch?v=-sfiReUu3o0)
- [Emergence & Systems Thinking — Systems Innovation Network](https://www.youtube.com/watch?v=KN6SaRmF_8c)

**Exercise — 25 min**

Choose one messy system you know well: a software team, household finances, traffic, your project backlog, housing prices, or something similar.

Write:

```text
System:
What behaviour am I trying to understand?
Elements:
Relationships:
System boundary:
What emerges that no individual element intends?
```

**Done when:** You can describe the problem without reducing it to one cause.

## 2. Behaviour over time — 60 min

**Watch**

- [System Dynamics: Systems Thinking and Modeling for a Complex World — MIT OpenCourseWare](https://www.youtube.com/watch?v=o-Yp8A7BPE8) — watch the introductory event–pattern–structure sections first.

**Exercise — 30 min**

For your system, draw 3–5 **behaviour-over-time graphs**.

Example:

```text
unfinished work
^
|       /\/\
|    __/    \___
|___/
+---------------> time
```

Do not explain them yet. Describe **what actually happens over time**.

**Done when:** You have moved from “something happened” to “there is a recurring pattern.”

## 3. Feedback loops — 90 min

**Watch**

- [Introduction to System Dynamics: Causal Loop Diagrams — transentis](https://www.youtube.com/watch?v=V3pPQk5Opc8)
- Continue the relevant feedback-loop section of the [MIT workshop](https://www.youtube.com/watch?v=o-Yp8A7BPE8).

Learn:

- reinforcing loops **R**;
- balancing loops **B**;
- causal direction;
- delays;
- circular rather than linear causality.

**Exercise — 40 min**

Create a causal-loop diagram containing:

- 6–12 variables;
- at least one reinforcing loop;
- at least one balancing loop;
- at least one delay.

Then ask: **Which loop currently dominates the system's behaviour?**

Optional tool: [Kumu system mapping guide](https://docs.kumu.io/disciplines/system-mapping).

## 4. Stocks, flows, and accumulation — 90 min

Do not skip this step. A lot of lightweight systems-thinking material stops at drawing arrows; system dynamics forces you to explain how quantities actually change.

**Watch**

- [Introduction to Stock and Flow Diagrams — Don Woodlock](https://www.youtube.com/watch?v=c27Rbmix6sE)
- Continue the stock-and-flow sections of the [MIT workshop](https://www.youtube.com/watch?v=o-Yp8A7BPE8).

**Exercise — 45 min**

Find one accumulating quantity in your system.

Examples:

```text
Backlog = incoming work − completed work
Savings = income − spending
Population = births − deaths
Trust = trust-building interactions − trust-damaging interactions
```

Draw the stock and its inflows and outflows. Then predict what happens if you change each flow independently.

**Done when:** You stop confusing a stock with the rate changing it.

## 5. Build a dynamic model — 60 min

Use [Loopy](https://ncase.me/loopy/) for a deliberately simple first simulation.

Recreate your causal model and run at least four experiments:

```text
baseline
increase A
decrease A
introduce or change a delay
```

Before each run, **predict the result first**.

| Change | Prediction | Actual result |
| --- | --- | --- |
| A ↑ | … | … |
| A ↓ | … | … |
| delay ↑ | … | … |

The prediction error is the useful part.

## 6. Recognise recurring structures — 75 min

Return to the MIT material instead of collecting dozens of superficial “systems archetypes” videos.

**Watch**

- Relevant archetype and example sections in [MIT — Systems Thinking and Modeling for a Complex World](https://www.youtube.com/watch?v=o-Yp8A7BPE8).

Learn to recognise at least:

- limits to growth;
- fixes that fail;
- shifting the burden;
- success to the successful;
- escalation.

Try to match your system to an archetype, then deliberately try to **disprove the match**. If the causal structure does not fit, reject the archetype.

**Done when:** Archetypes become hypotheses, not labels.

## 7. Intervention and leverage — 75 min

Now—and only now—ask how to change the system.

**Watch**

- [Leverage Points: Places to Intervene in a System](https://www.youtube.com/watch?v=VvrUt9zYxKk)

**Read**

- [Donella Meadows — Leverage Points: Places to Intervene in a System](https://donellameadows.org/archives/leverage-points-places-to-intervene-in-a-system/)

Generate **five interventions** for your system and rank them:

```text
intervention
↓
mechanism
↓
loop or stock affected
↓
expected behaviour change
↓
likely unintended consequence
```

Pick **one**, not five.

## 8. Capstone: explain a system — 2 hours

Create a one-page systems analysis of a real problem. Include:

```text
1. Problem or question
2. System boundary
3. 2–3 behaviour-over-time graphs
4. Causal-loop diagram
5. Important stocks and flows
6. Delays
7. Dominant feedback loops
8. Possible archetype
9. Three leverage points
10. One intervention worth testing
11. What evidence could prove the model wrong?
```

Use [Kumu](https://kumu.io/) if the map becomes too large for paper.

**Final test:** Give the page to someone unfamiliar with the problem. Can they explain **why the observed behaviour emerges**?

## The sequence

```text
Parts
  ↓
Relationships
  ↓
Behaviour over time
  ↓
Feedback
  ↓
Stocks and flows
  ↓
Delays
  ↓
System structure
  ↓
Archetypes
  ↓
Leverage
  ↓
Intervention
```

Resist adding more videos. The danger with systems thinking is becoming fluent in words like *emergence*, *feedback*, and *leverage* without ever building a falsifiable model. After approximately ten hours, another twenty hours of video will teach less than modelling five messy real systems yourself.
