# Practical Systems Thinking

> This curriculum was developed with AI assistance and has not been independently validated.

**Goal:** Learn to explain how a system's structure generates behaviour, build and test a small stock-and-flow model, and design one evidence-based intervention experiment.

**Level:** Beginner. No previous modelling experience is required.

**Total:** Approximately 10.5 hours of work, or 10–12 hours including setup and breaks.

| Section | Time |
| --- | ---: |
| 1. Frame the system | 45 min |
| 2. Describe behaviour over time | 60 min |
| 3. Map feedback | 90 min |
| 4. Model stocks and flows | 90 min |
| 5. Build and test a simulation | 90 min |
| 6. Test recurring structures | 60 min |
| 7. Choose an intervention experiment | 75 min |
| 8. Capstone | 120 min |

## How to use this curriculum

Use two systems throughout:

1. Read the **project-backlog reference case** to see what each technique should produce.
2. Apply the technique to one real system you know and can investigate.

Choose a real system with:

- behaviour that changes over weeks, months, or years;
- at least one accumulating quantity you can measure or estimate;
- some historical evidence, even if incomplete;
- a boundary small enough to model in a few variables.

Mark every important statement as **observed**, **estimated**, or **assumed**. A plausible story is not evidence.

Do not force a feedback loop, archetype, or intervention to fit. Record when the evidence does not support one.

## Core resources and tools

- **Core lecture:** [System Dynamics: Systems Thinking and Modeling for a Complex World — MIT OpenCourseWare](https://www.youtube.com/watch?v=o-Yp8A7BPE8). Each section below specifies a short excerpt. An [official transcript is available as a PDF](https://ocw.mit.edu/courses/res-15-004-system-dynamics-systems-thinking-and-modeling-for-a-complex-world-january-iap-2020/0c69abc4986594e01df51c597cadc689_o-Yp8A7BPE8.pdf).
- **Qualitative mapping:** Paper is enough. [Loopy](https://ncase.me/loopy/) is optional for exploring simple circles-and-arrows models.
- **Stock-and-flow simulation:** Use the free browser-based [Insight Maker](https://www.insightmaker.com/) and its [system-dynamics guide](https://www.insightmaker.com/docs/systemdynamics). [Vensim Personal Learning Edition](https://vensim.com/vensim-personal-learning-edition/) is a free alternative for personal or educational use.
- **Large final maps:** [Kumu](https://kumu.io/) is optional. Its [system-mapping guide](https://docs.kumu.io/disciplines/system-mapping) explains causal links, loops, and delay markings.

## Reference case: a growing project backlog

Use this deliberately small example to check your work.

| Item | Reference-case answer |
| --- | --- |
| Question | Why is unfinished work growing even though the team completes work every week? |
| Time horizon | The previous 12 weeks |
| Boundary | Work from commitment through completion; team capacity, work-in-progress policies, and prioritisation |
| Outside boundary | How customers generate requests and how staffing budgets are set |
| Main stock | Unfinished work, measured in tasks |
| Evidence to seek | Weekly unfinished, accepted, and completed task counts; lead time; staffing changes |
| Initial hypothesis | Work enters faster than it leaves, while congestion reduces effective completion capacity |

The numbers used below are illustrative, not empirical evidence.

## 1. Frame the system — 45 min

### Watch — 13 min

- [Open-loop and closed-loop thinking, then structure generating behaviour — MIT, 10:56–23:59](https://www.youtube.com/watch?v=o-Yp8A7BPE8&t=656s)

### Exercise — 30 min

Write:

```text
Question:
Behaviour I want to explain:
Time horizon:
Inside the boundary:
Outside the boundary:
People affected:
Evidence I already have:
Evidence I still need:
Important assumptions:
```

Phrase the question as behaviour over time, not as blame. Prefer “Why has delivery time risen during the last six months?” over “Why is the team inefficient?”

### Check your work

- The question names a variable and a time horizon.
- The boundary says what is excluded as well as included.
- The system is small enough to represent with roughly 6–12 variables.
- At least one relevant person could disagree with your boundary.
- Observations and assumptions are distinguishable.

**Done when:** Someone else can tell what behaviour the model must explain and what the model deliberately omits.

## 2. Describe behaviour over time — 60 min

A **behaviour-over-time graph** is a sketch or plot of how one variable changes across the chosen time horizon. It is also called a **reference mode** because it states the behaviour the model should reproduce.

### Reference case: behaviour over time

Suppose records show unfinished work rising from 40 to 64 tasks over eight weeks, with short plateaus. Draw that pattern before explaining it. Draw separate graphs for incoming work, completed work, and lead time.

### Exercise: draw the reference modes

Draw two or three behaviour-over-time graphs for your system.

For every graph:

- label both axes and include units;
- show the relevant time horizon;
- cite the data source, or label the shape **estimated** or **assumed**;
- note discontinuities or uncertainty;
- describe the pattern without explaining its cause.

Use a table first if you have data:

| Week | Unfinished work (tasks) | Incoming work (tasks/week) | Completed work (tasks/week) |
| ---: | ---: | ---: | ---: |
| 0 | 40 | — | — |
| 1 | 43 | 18 | 15 |
| 2 | 46 | 18 | 15 |
| … | … | … | … |

**Common error:** Drawing a desired future rather than the observed past. Put desired behaviour on a separate graph.

**Done when:** The graphs define the behaviour the later model must explain, including units, time horizon, evidence, and uncertainty.

## 3. Map feedback — 90 min

A **causal-loop diagram** is a qualitative map of variables connected by causal links.

### Watch — 10 min

- [Causal links, loop polarity, and feedback — MIT, 24:01–33:25](https://www.youtube.com/watch?v=o-Yp8A7BPE8&t=1441s)

### Notation

- `A +→ B` means that, all else equal, more A produces more B than otherwise, and less A produces less B than otherwise.
- `A −→ B` means that, all else equal, more A produces less B than otherwise, and less A produces more B than otherwise.
- **R** marks a reinforcing loop that amplifies change.
- **B** marks a balancing loop that opposes change or moves towards a goal.
- Two short parallel lines on a link mark a material delay.

Polarity does not mean that two variables happen to move together in the historical data. It states a causal claim under otherwise equal conditions.

### Reference case: feedback

```text
B1 — workload response
unfinished work +→ delivery pressure +→ overtime
overtime +→ completion rate −→ unfinished work

R1 — congestion
unfinished work +→ concurrent work +→ context switching
context switching +→ completion time +→ unfinished work
```

The reference case contains one balancing loop and one reinforcing loop. Your system may not.

### Exercise: build the causal-loop diagram

Create a causal-loop diagram with roughly 6–12 variables.

For each variable and link:

1. Name the variable as a quantity that can rise or fall. Use “delivery pressure,” not “apply pressure.”
2. State the link as a sentence: “If A increases, B will be higher/lower than otherwise because …”
3. Mark the polarity.
4. Mark important delays.
5. Attach evidence or mark the link as assumed.
6. Trace each closed loop and calculate whether it is reinforcing or balancing.

Then identify which supported loop best explains each behaviour-over-time graph. Do not add a loop merely to satisfy the exercise.

### Causal-loop checklist

- Every link has an unambiguous direction and polarity.
- No link changes polarity under ordinary conditions; if it does, add a missing intermediate variable or narrow the conditions.
- Each loop tells a complete causal story when read around the circle.
- Important external drivers are shown as external rather than quietly treated as feedback.
- Correlation alone is not presented as causation.

**Done when:** Another person can read each loop as a causal argument and identify which links are evidence-backed or assumed.

## 4. Model stocks and flows — 90 min

A **stock** is a quantity accumulated over time. A **flow** is a rate that changes a stock per unit of time.

### Watch — 6 min

- [Stocks, flows, and accumulation — MIT, 33:25–39:26](https://www.youtube.com/watch?v=o-Yp8A7BPE8&t=2005s)

The core relationship is:

```text
change in stock per unit time = total inflow rate − total outflow rate

stock(t) = initial stock
           + accumulated inflows from time 0 to t
           − accumulated outflows from time 0 to t
```

Do not write `Backlog = incoming work − completed work`. The right-hand side contains rates; it describes the backlog's rate of change, not its level.

### Reference case: stock and flow

```text
Stock: unfinished work [tasks]
Initial value: 40 tasks
Inflow: work intake [tasks/week] = 18
Outflow: work completion [tasks/week] = 15

change in unfinished work [tasks/week]
  = work intake [tasks/week] − work completion [tasks/week]

after 4 weeks:
  unfinished work = 40 tasks + (18 − 15 tasks/week) × 4 weeks
                  = 52 tasks
```

### Exercise: define the stock and flows

Choose one important stock in your system and record:

| Field | Your answer |
| --- | --- |
| Stock name and unit | |
| Initial value and source | |
| Inflow names and units | |
| Outflow names and units | |
| Time unit | |
| Equation or update rule | |
| Assumptions | |

Draw the stock, inflows, outflows, and the variables that control each flow. Predict what happens when each flow changes independently.

### Stock-and-flow checklist

- The stock is measurable at one instant.
- Every flow uses “stock units per time unit.”
- The equation is dimensionally consistent: units match on both sides.
- A stock changes only through its flows.
- The initial value is explicit.
- A soft quantity such as trust is operationally defined before being treated as a stock.

**Done when:** You can explain the difference between the stock level, its inflow and outflow rates, and its net rate of change.

## 5. Build and test a simulation — 90 min

Use [Insight Maker](https://www.insightmaker.com/) or Vensim Personal Learning Edition to create a small stock-and-flow simulation. Loopy is useful for qualitative exploration but does not replace this step.

### Build

1. Add the stock, its initial value, and its unit.
2. Add its inflows and outflows with units per time.
3. Add the variables needed to calculate the flows.
4. Set the simulation horizon to match your behaviour-over-time graphs.
5. Run the baseline and compare its shape with the reference mode.

### Test

Predict each result before running it:

| Experiment | Prediction and reason | Actual result | What the difference taught me |
| --- | --- | --- | --- |
| Baseline | | | |
| Inflow increased 20% | | | |
| Outflow capacity increased 20% | | | |
| Initial stock doubled | | | |
| One assumption or delay changed | | | |

### Challenge the model

- **Units check:** Do all equations use compatible units?
- **Extreme-condition test:** What happens when an inflow or outflow is zero? Can a stock become impossibly negative?
- **Structure check:** Does every equation correspond to a causal claim you can explain?
- **Behaviour check:** Can the model reproduce the broad historical pattern without implausible parameter values?
- **Sensitivity check:** Does a small assumption change completely reverse the conclusion?

A model is not validated merely because it runs. Record mismatches, revise one assumption at a time, and keep the failed predictions.

**Done when:** The model is dimensionally consistent, survives simple extreme-condition tests, and either reproduces the reference mode or clearly documents why it does not.

## 6. Test recurring structures — 60 min

A **system archetype** is a recurring causal structure. Treat it as a hypothesis, not a label.

This course assesses only two:

- **Limits to growth:** A reinforcing process creates growth, then a balancing process slows it as a constraint becomes important.
- **Fixes that fail:** A corrective action improves a symptom in the short term, but a delayed consequence makes the original problem worse.

Other useful archetypes—shifting the burden, success to the successful, and escalation—are follow-on material, not requirements for this course.

### Exercise: test the archetypes

For each of the two archetypes:

1. Compare its loops with your causal-loop diagram.
2. Identify the exact variables and links that would have to correspond.
3. Name evidence that supports the match.
4. Name evidence that would disprove the match.
5. Reject the archetype if the causal structure does not fit.

It is acceptable to conclude that neither archetype applies.

**Done when:** You can defend or reject an archetype using causal structure and evidence rather than resemblance or vocabulary.

## 7. Choose an intervention experiment — 75 min

Now—and only now—ask how to change the system.

### Read

- [Donella Meadows — Leverage Points: Places to Intervene in a System](https://donellameadows.org/archives/leverage-points-places-to-intervene-in-a-system/)

Generate five possible interventions. Describe the mechanism before judging the idea:

```text
intervention
↓
changed rule, information link, flow, stock, delay, goal, or feedback loop
↓
expected change in behaviour over time
↓
possible delayed or unintended consequences
```

Compare the interventions:

| Intervention | Loop or stock affected | Evidence for mechanism | Expected impact | Time to effect | Reversible? | Feasibility | Main risk |
| --- | --- | --- | --- | --- | --- | --- | --- |
| | | | low/medium/high | | yes/no | low/medium/high | |

Choose one **small, reversible experiment**, not an immediate full rollout. Specify:

```text
Change to test:
People affected:
Expected behaviour:
Leading indicator:
Failure or stop condition:
Review date:
Evidence that would change my mind:
```

Do not assume that a higher-ranked leverage point is automatically practical or ethical. State who benefits, who bears the risk, and who should participate in the decision.

**Done when:** The chosen experiment has an explicit causal mechanism, measurement plan, stop condition, and account of affected people.

## 8. Capstone: explain and challenge a system — 2 hours

Create a two-page analysis plus a one-page model appendix.

### Page 1 — Behaviour and evidence

1. Problem question, time horizon, and system boundary
2. Two or three behaviour-over-time graphs
3. Evidence sources, uncertainties, and important assumptions

### Page 2 — Structure and action

1. Causal-loop diagram and dominant supported loops
2. Important stock, flows, delays, and units
3. Archetype match or explicit rejection
4. Three candidate interventions
5. One intervention experiment and its stop condition
6. Evidence that could prove the explanation wrong

### Model appendix

1. Stock-and-flow diagram and equations
2. Initial values, units, parameter sources, and assumptions
3. Prediction-versus-result experiment table
4. Failed tests, limitations, and unresolved questions

Use Kumu if the causal map becomes too large for paper, but simplify the map before adding more variables.

### Self-assessment rubric

Score each criterion 0, 1, or 2:

- **0:** absent or technically incorrect
- **1:** present but incomplete, weakly supported, or unclear
- **2:** correct, explicit, evidence-backed, and understandable

| Criterion | Score |
| --- | ---: |
| Question, boundary, and time horizon are precise | /2 |
| Behaviour-over-time graphs have units, sources, and uncertainty | /2 |
| Causal links and loop polarities are defensible | /2 |
| Stocks, flows, equations, initial values, and units are correct | /2 |
| Simulation predictions, tests, and revisions are documented | /2 |
| Intervention follows from the model and includes risks and measures | /2 |
| Limitations and possible falsifying evidence are explicit | /2 |
| **Total** | **/14** |

Revise the work if the total is below 11 or if causal logic, stock-and-flow correctness, or model testing receives 0.

**Final test:** Give the analysis to someone unfamiliar with the problem. Ask them:

1. What behaviour is this trying to explain?
2. Why does the model say that behaviour emerges?
3. Which claims are evidence-backed and which are assumptions?
4. What intervention is being tested, and what could make the test stop?
5. What evidence could show that the model is wrong?

If they cannot answer, simplify or revise the analysis.

## The sequence

```text
Question and boundary
  ↓
Behaviour over time
  ↓
Feedback structure
  ↓
Stocks, flows, and delays
  ↓
Simulation and challenge tests
  ↓
Archetype as a hypothesis
  ↓
Leverage and intervention experiment
  ↓
Evidence, revision, or rejection
```

Resist adding more videos. After this course, modelling several different real systems—and finding where each model fails—will teach more than collecting additional terminology.
