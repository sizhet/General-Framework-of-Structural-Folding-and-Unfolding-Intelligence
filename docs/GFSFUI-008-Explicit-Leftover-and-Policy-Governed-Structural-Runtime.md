# GFSFUI-008 — Explicit Leftover and Policy-Governed Structural Runtime

## Two Runtime Principles for Reliable Structural Folding and Unfolding

**Series:** General Framework of Structural Folding and Unfolding Intelligence (GFSFUI)
**Document:** GFSFUI-008
**Version:** v1.0.0
**Date:** 2026-09-07

---

## Abstract

A structural Fold/Unfold framework can be misunderstood in two seemingly natural ways.

The first misunderstanding is to assume that every object, observation, query, or candidate must eventually be assigned to an existing structural branch.

The second is to assume that once structural evidence has been obtained, the runtime should directly act on that evidence.

Both assumptions are unsafe.

Real-world data are noisy, incomplete, ambiguous, novel, and frequently outside the reliable coverage of the current structural representation. A structural runtime therefore requires an explicit **Leftover branch** at major processing stages. Leftover is not merely failure or garbage. It represents what the current system should not yet force into a certified structure.

Likewise, structural evidence does not itself determine action. Decisions depend on goals, risk tolerance, cost, latency, user preference, operational state, and governance constraints. These belong to a distinct **Policy layer**.

This document introduces two complementary runtime principles:

> **Principle I — Explicit Leftover:**
> Every major structural transformation should permit an explicit branch for what it cannot yet reliably fold, localize, unfold, or certify.

and:

> **Principle II — Policy-Governed Runtime:**
> Structural intelligence defines a possibility space; policy governs how that space is searched, accepted, rejected, deferred, escalated, unfolded, and evolved.

Together, these principles extend the Fold/Unfold framework from a structural representation mechanism toward a controllable, uncertainty-aware, and user-tunable structural runtime.

---

# 1. Why This Clarification Is Necessary

The basic GFSFUI lifecycle can be summarized as:

$$
\text{Represent}
\rightarrow
\text{Fold}
\rightarrow
\text{Localize}
\rightarrow
\text{Search}
\rightarrow
\text{Unfold}
\rightarrow
\text{Validate}
\rightarrow
\text{Grow}
\rightarrow
\text{Refold}
$$

This formulation is intentionally compact.

However, a compact pipeline can create a dangerous implementation impression:

> every input enters a stage, receives a structural answer, and proceeds to the next stage.

Real-world structural intelligence cannot safely operate this way.

At almost every stage, the system may encounter something that should **not** be forced forward.

Likewise, the arrows in the lifecycle should not be interpreted as unconditional transitions.

Many transitions are governed by policy.

A more realistic view is therefore:

$$
\boxed{
\text{Structural Space}
+
\text{Leftover Space}
+
\text{Policy Space}
}
$$

These three spaces play different roles.

* **Structural Space** represents known structural possibilities.
* **Leftover Space** preserves what is not yet reliably represented.
* **Policy Space** governs how the runtime operates across both.

---

# 2. Misunderstanding I — Everything Must Be Folded

Suppose a set of observations is:

$$
X = \{x_1,x_2,\ldots,x_n\}
$$

A naive structural implementation may attempt to guarantee:

$$
\forall x\in X,\quad x\rightarrow CCC_i
$$

for some existing structural class, branch, cluster, CCC, or structural memory unit.

This creates a hidden assumption:

> the current structural system already contains an adequate destination for every object.

In open-world environments, this assumption is usually false.

An object may be:

* noisy,
* incomplete,
* ambiguous,
* weakly supported,
* structurally unusual,
* genuinely novel,
* temporarily irrelevant,
* outside current MET capability.

Forcing such an object into an existing structure may increase nominal coverage while reducing structural truthfulness.

Therefore:

$$
\boxed{
Not\ Everything\ Should\ Be\ Folded
}
$$

---

# 3. Explicit Leftover

A more realistic structural decomposition is:

$$
X
=
Folded(X)
\cup
Leftover(X)
$$

where:

$$
Leftover(X)
=
Noise
\cup
Uncertain
\cup
Outlier
\cup
Novel
\cup
Deferred
$$

These categories should not necessarily be implemented as five rigid classes.

They describe different reasons why an object may remain outside the currently accepted Fold.

### Noise

The observation may contain insufficient useful structure.

### Uncertain

The system may see plausible structural destinations but lack sufficient confidence to accept one.

### Outlier

The observation may be valid but structurally distant from established groups.

### Novel

The observation may represent a genuinely new structural pattern.

### Deferred

The observation may be potentially useful, but current cost, policy, priority, or runtime conditions do not justify further processing.

This leads to a fundamental distinction:

$$
\boxed{
Leftover \neq Failure
}
$$

Leftover may instead represent disciplined structural restraint.

---

# 4. Forced Folding Is a Structural Error

Suppose localization produces a structural score:

$$
S(x,CCC_i)
$$

A forced classifier may select:

$$
CCC^*
=
\arg\max_i S(x,CCC_i)
$$

regardless of the absolute quality of the match.

A structural runtime should instead be allowed to use an acceptance policy:

$$
x
\rightarrow
\begin{cases}
CCC^*, & S(x,CCC^*) \ge T_{accept}\\
Leftover, & S(x,CCC^*) < T_{accept}
\end{cases}
$$

The important distinction is that:

$$
Best\ Available
\neq
Good\ Enough
$$

An object can have a nearest structural destination while still being too far away to justify assignment.

If the runtime ignores this distinction, it can produce:

$$
Forced\ Folding
\rightarrow
CCC\ Contamination
\rightarrow
Poor\ Localization
\rightarrow
Poor\ Unfolding
$$

The error then propagates through the Fold/Unfold lifecycle.

---

# 5. Leftover Should Exist at Multiple Layers

Leftover should not be implemented only as a final exception handler.

It should be available wherever structural confidence can legitimately fail.

For example:

$$
Raw\ Objects
\rightarrow
Fold
\rightarrow
\begin{cases}
Structural\ Memory\\
Leftover_F
\end{cases}
$$

During localization:

$$
Query
\rightarrow
Localization
\rightarrow
\begin{cases}
Candidate\ CCC\\
Leftover_L
\end{cases}
$$

During unfolding:

$$
Core + Requirement
\rightarrow
Unfold
\rightarrow
\begin{cases}
Candidate\ Structure\\
Leftover_U
\end{cases}
$$

During validation:

$$
Candidate
\rightarrow
Validation
\rightarrow
\begin{cases}
Certified\\
Rejected\\
Leftover_V
\end{cases}
$$

Therefore:

$$
\boxed{
Every\ Major\ Structural\ Layer
Should\ Permit\ an\ Escape\ Branch
}
$$

The exact form of that branch depends on the application.

---

# 6. Leftover as a MET Boundary

A large Leftover set does not automatically imply that the framework is wrong.

It may indicate that the current MET is immature.

Early structural systems may have:

$$
Low\ Reliable\ Coverage
$$

and therefore:

$$
Large\ Leftover
$$

As representation, metrics, CCC construction, retrieval, localization, validation, and policy improve:

$$
MET(t)\uparrow
$$

the runtime may achieve:

$$
Reliable\ Coverage(t)\uparrow
$$

and some previously unresolved Leftovers may become structurally manageable.

Thus:

$$
Leftover(t)
$$

can reveal the evolving boundary of current structural competence.

This suggests a useful engineering concept:

$$
\boxed{
Leftover\ Frontier
}
$$

The Leftover Frontier separates what the current runtime can reliably structuralize from what it cannot yet reliably handle.

---

# 7. The Leftover Curve Is Not a Standalone Optimization Target

It is tempting to define progress simply as:

$$
Leftover\ Rate\downarrow
$$

This is insufficient.

A system can trivially reduce Leftover by lowering acceptance standards.

For example:

$$
T_{accept}\downarrow
$$

may produce:

$$
Coverage\uparrow
$$

while simultaneously causing:

$$
False\ Folding\uparrow
$$

Therefore, structural progress should consider several quantities together:

$$
Reliable\ Coverage\uparrow
$$

$$
False\ Folding\downarrow
$$

$$
Validation\ Success\uparrow
$$

$$
Unnecessary\ Escalation\downarrow
$$

$$
Useful\ Leftover\ Resolution\uparrow
$$

The objective is not:

> eliminate Leftover.

The objective is:

> expand reliable structural coverage without destroying structural honesty.

---

# 8. Leftover Can Become Future Structure

One of the most important properties of Leftover is that it need not remain Leftover forever.

Repeated unresolved cases may reveal:

$$
Leftover
\rightarrow
Repeated\ Difference
\rightarrow
Candidate\ Delta
$$

which may lead to:

$$
Candidate\ Delta
\rightarrow
Validation
\rightarrow
New\ Branch
$$

or:

$$
Candidate\ Delta
\rightarrow
New\ CCC
$$

or eventually:

$$
Candidate\ Delta
\rightarrow
Specialist
\rightarrow
Brain\ Unit
$$

Thus Leftover can participate directly in structural continual learning.

A useful lifecycle is:

$$
\boxed{
Leftover
\rightarrow
Accumulate
\rightarrow
Compare
\rightarrow
Discover\ Delta
\rightarrow
Validate
\rightarrow
Grow
\rightarrow
Refold
}
$$

This converts unresolved experience into a source of structural evolution.

---

# 9. Misunderstanding II — Evidence Directly Determines Action

A second common misunderstanding is:

$$
Structural\ Evidence
\rightarrow
Decision
$$

This collapses two fundamentally different problems.

Structural intelligence may determine:

* what patterns exist,
* what structures are similar,
* what CCCs are plausible,
* what alternatives are available,
* what historical evidence is relevant,
* what candidate unfoldings are structurally possible.

But none of these alone determines what should be done.

The same structural evidence may lead to different actions under different:

* goals,
* risk profiles,
* budgets,
* latency requirements,
* safety requirements,
* user preferences,
* organizational rules,
* operating environments.

Therefore:

$$
\boxed{
Structural\ Evidence
\neq
Policy
\neq
Decision
}
$$

---

# 10. Structural Space and Policy Space

The distinction can be expressed as two complementary spaces.

## Structural Space

Structural Space answers:

> **What structural possibilities exist?**

It may contain:

$$
CCC_1,CCC_2,\ldots,CCC_n
$$

candidate branches, alternative explanations, historical analogues, CallingGraphs, structural memories, or possible unfolding paths.

## Policy Space

Policy Space answers:

> **Given the current goal and operating conditions, what should the runtime do with those possibilities?**

A simplified relationship is:

$$
Structural\ Space
\xrightarrow{Policy}
Runtime\ Action
$$

Policy therefore does not replace structural intelligence.

It governs its use.

---

# 11. Policy Exists Throughout the Runtime

Policy should not be understood only as the final decision layer.

Policy decisions may exist throughout the Fold/Unfold lifecycle.

### Folding Policy

$$
Object
\xrightarrow{Policy}
\begin{cases}
Accept\ Fold\\
Leftover
\end{cases}
$$

Questions include:

* What similarity is sufficient?
* How much structural difference is acceptable?
* Should alternatives be preserved?
* When should a new branch be created?

### Localization Policy

$$
Query
\xrightarrow{Policy}
\begin{cases}
Top1\\
TopK\\
Multi\text{-}Branch\\
Leftover\\
Escalate
\end{cases}
$$

Questions include:

* How wide should retrieval be?
* How strict should verification be?
* Should competing CCCs remain active?

### Unfolding Policy

$$
Certified\ Core + Requirement
\xrightarrow{Policy}
Unfolding\ Budget
$$

Questions include:

* How much of the structure may change?
* How much Delta is permitted?
* How many candidate unfoldings should be explored?
* When should existing structure be reused rather than regenerated?

### Validation Policy

$$
Candidate
\xrightarrow{Policy}
\begin{cases}
Certify\\
Reject\\
Retest\\
Escalate\\
Leftover
\end{cases}
$$

Questions include:

* What evidence is sufficient?
* How many tests are required?
* What failure rate is acceptable?
* When is human review required?

---

# 12. Policy Governs the Leftover Branch

Leftover is where Policy becomes especially important.

An unresolved object does not imply one universal response.

A policy may choose:

$$
Leftover
\xrightarrow{Policy}
\begin{cases}
Ignore\\
Store\\
Defer\\
Search\\
Retrieve\ Wider\\
Call\ LLM\\
Request\ Human\\
Run\ Experiment\\
Create\ Candidate\ Branch\\
Trigger\ Structural\ Growth
\end{cases}
$$

Different environments may select very different actions for the same structural uncertainty.

For example:

A low-cost exploratory system may prefer:

$$
Leftover\rightarrow Search
$$

A safety-critical system may prefer:

$$
Leftover\rightarrow Human\ Review
$$

A continual-learning system may prefer:

$$
Repeated\ Leftover
\rightarrow
Candidate\ Structural\ Growth
$$

Thus:

$$
\boxed{
Leftover\ Defines\ Unresolved\ Structure;
Policy\ Determines\ What\ Happens\ Next
}
$$

---

# 13. Policy Profiles

Because Policy is separate from Structural Space, the same structural runtime can support multiple operational profiles.

For example:

$$
Policy_{safe}
$$

may favor:

* higher acceptance thresholds,
* wider validation,
* more escalation,
* smaller unfolding Delta.

While:

$$
Policy_{exploratory}
$$

may favor:

* broader search,
* more candidate branches,
* greater novelty tolerance,
* faster structural experimentation.

Other possible profiles include:

$$
Policy_{low-cost}
$$

$$
Policy_{low-latency}
$$

$$
Policy_{high-confidence}
$$

$$
Policy_{aggressive-growth}
$$

The underlying structural memory does not necessarily need to change.

This separation is important because:

$$
User\ Preference
\neq
Structural\ Truth
$$

and:

$$
Operational\ Policy
\neq
Structural\ Evidence
$$

---

# 14. Toward User-Tunable Structural Runtime

This separation creates a significant engineering opportunity.

Traditional AI customization often focuses on changing:

* prompts,
* training data,
* model parameters,
* fine-tuning.

A structural runtime introduces another control surface.

The user may configure:

* Fold thresholds,
* Leftover tolerance,
* retrieval width,
* verification strictness,
* novelty sensitivity,
* search budget,
* Unfold Delta budget,
* validation requirements,
* risk profile,
* cost limits,
* latency limits,
* escalation rules,
* human-review thresholds.

Thus the user may increasingly:

$$
\boxed{
Configure\ the\ Structural\ Runtime
}
$$

rather than retrain the underlying intelligence.

This creates a natural interface between GFSFUI and policy-oriented runtime systems such as PDS.

---

# 15. PDS as a Governance Layer

Within a larger Structural Intelligence architecture, a Policy Decision System (PDS) can serve as a governance mechanism over structural runtime choices.

The relationship can be summarized as:

$$
GFSFUI
\rightarrow
Structural\ Possibility\ Space
$$

while:

$$
PDS
\rightarrow
Policy\ Selection\ and\ Runtime\ Governance
$$

Together:

$$
\boxed{
Structural\ Possibilities
+
Policy\ Governance
\rightarrow
Controlled\ Intelligence
}
$$

This division is especially important in systems where the same structural knowledge must support different users, environments, risk levels, or operational goals.

Policy therefore becomes a control plane over Fold/Unfold operations rather than merely a final decision rule.

---

# 16. A More Complete Fold/Unfold Runtime

With Explicit Leftover and Policy Governance included, the basic GFSFUI lifecycle becomes more realistic.

Instead of:

$$
Input
\rightarrow
Fold
\rightarrow
Localize
\rightarrow
Unfold
\rightarrow
Output
$$

we obtain:

$$
Input
\rightarrow
Fold
\rightarrow
\begin{cases}
Structural\ Memory\\
Leftover
\end{cases}
$$

followed by:

$$
Query
\rightarrow
Policy\text{-}Governed\ Localization
\rightarrow
\begin{cases}
Candidate\ Structure\\
Leftover
\end{cases}
$$

then:

$$
Certified\ Core + Requirement
\rightarrow
Policy\text{-}Governed\ Unfold
\rightarrow
\begin{cases}
Candidate\\
Leftover
\end{cases}
$$

and:

$$
Candidate
\rightarrow
Policy\text{-}Governed\ Validation
\rightarrow
\begin{cases}
Certified\\
Rejected\\
Deferred\\
Escalated
\end{cases}
$$

Finally:

$$
Validated\ Experience
\rightarrow
Refold
\rightarrow
Structural\ Growth
$$

This produces a broader runtime loop:

$$
\boxed{
Experience
\rightarrow
Fold
\rightarrow
Structural\ Memory
\rightarrow
Localize
\rightarrow
Unfold
\rightarrow
Validate
\rightarrow
Refold
}
$$

with two persistent control dimensions:

$$
\boxed{Leftover}
$$

and:

$$
\boxed{Policy}
$$

---

# 17. Three-Space View of Structural Intelligence

The resulting architecture can be summarized through three spaces.

## 17.1 Structural Space

Contains what the system currently knows how to represent structurally.

Examples:

* CCCs,
* structural memories,
* CallingGraphs,
* Difference Branches,
* candidate trajectories,
* structural alternatives.

---

## 17.2 Leftover Space

Contains what the current system should not yet force into established structure.

Examples:

* uncertainty,
* novelty,
* weak evidence,
* unresolved differences,
* unsupported candidates,
* deferred cases.

---

## 17.3 Policy Space

Controls runtime behavior across Structural Space and Leftover Space.

Examples:

* thresholds,
* search width,
* budgets,
* risk tolerance,
* escalation,
* validation requirements,
* growth rules,
* user profiles.

Thus:

$$
\boxed{
Structural\ Intelligence
\approx
Structural\ Space
+
Leftover\ Space
+
Policy\text{-}Governed\ Runtime
}
$$

This is not intended as a mathematical identity.

It is an architectural decomposition.

---

# 18. Engineering Implications

These two principles create several concrete MET directions.

### Leftover Management MET

How should unresolved cases be stored, indexed, aged, compared, and revisited?

### Adaptive Threshold MET

Can acceptance thresholds evolve according to validation history and operating context?

### Structural Coverage MET

How should reliable coverage be measured without rewarding forced classification?

### Policy Profile MET

How should safe, exploratory, low-cost, high-confidence, and other profiles be represented?

### Escalation MET

When should the runtime escalate to:

* broader search,
* an LLM,
* another Brain Unit,
* an experiment,
* a human?

### Policy Learning MET

Can successful runtime policy choices themselves be learned and Folded?

### Policy Certification MET

How can policy changes be tested before deployment?

### User Control MET

What minimal set of runtime controls gives users meaningful governance without exposing unnecessary structural complexity?

These questions connect Fold/Unfold intelligence directly to practical runtime engineering.

---

# 19. Two Canonical Principles

The central claims of this document can be compressed into two principles.

## Principle I — Explicit Leftover

> **Every major structural transformation should preserve an explicit branch for what it cannot yet reliably fold, localize, unfold, or certify.**

The system should be allowed to say:

> **Not yet structurally resolved.**

This is a capability, not an embarrassment.

---

## Principle II — Policy-Governed Runtime

> **Structural intelligence defines the possibility space; policy governs how that space is searched, accepted, rejected, deferred, escalated, unfolded, and evolved.**

The system should distinguish:

$$
Evidence
$$

from:

$$
Policy
$$

from:

$$
Decision
$$

---

# 20. Final Perspective

A mature structural intelligence system should not be required to understand everything.

Nor should it be allowed to act on everything it structurally recognizes.

These two restrictions are complementary.

Explicit Leftover prevents the runtime from pretending that its current structural model covers the entire world.

Policy Governance prevents the runtime from treating structural evidence as an automatic command.

Together:

$$
\boxed{
Leftover
\rightarrow
Respect\ the\ Unknown
}
$$

and:

$$
\boxed{
Policy
\rightarrow
Control\ the\ Known
}
$$

This produces a more realistic view of structural intelligence:

$$
\boxed{
Known\ Structure
+
Explicit\ Unknown
+
Governed\ Action
}
$$

The Fold/Unfold framework can therefore evolve not only by building better structural memory, but also by improving its ability to recognize its current boundaries and govern what happens at those boundaries.

That combination may be essential for scalable, controllable, and continually growing Structural Intelligence.

---

## Canonical Summary

```text
Experience
    |
    v
Represent
    |
    v
Fold ----------------------> Leftover
    |                           |
    v                           |
Structural Memory              |
    |                           |
    v                           |
Localize -------------------> Leftover
    |                           |
    v                           |
Candidate Structure            |
    |                           |
    v                           |
Policy-Governed Unfold -----> Leftover
    |
    v
Candidate
    |
    v
Validate -------------------> Reject / Defer / Escalate
    |
    v
Certified Experience
    |
    v
Refold / Grow
    |
    +-----------------------> Structural Memory


Across the runtime:

Structural Space
      +
Leftover Space
      +
Policy Space
      |
      v
Controlled Fold/Unfold Intelligence
```

---

## One-Sentence Takeaway

> **A reliable Fold/Unfold runtime must know what not to force into structure, and must use policy to govern what it does with the structure it has.**
