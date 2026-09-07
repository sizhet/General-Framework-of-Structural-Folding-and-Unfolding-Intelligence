# GFSFUI-002 — Generic Structural Folding: From Individuals to Structural Memory

**GFSFUI Series — General Framework of Structural Folding and Unfolding Intelligence**

**Document ID:** GFSFUI-002
**Status:** Core Framework Paper
**Version:** v1.0
**Language:** English

---

## Abstract

Structural Folding is the process by which a population of concrete individuals is transformed into reusable structural memory.

This paper develops the Folding side of the **General Framework of Structural Folding and Unfolding Intelligence (GFSFUI)**.

The framework begins with individuals represented through a **GenericContainerStarmap**. Meaningful metric or structural comparison is then used to identify shared structure, localize differences, construct Cluster-Central CCCs, organize Metric Differential structures, and attach specialized intelligence to structural nodes.

The central transformation is:

> **Individuals → Comparable Representations → Similarity → Shared Structure → Difference Localization → Dispatch → Structural Memory**

The resulting memory is not merely a compressed dataset. It may contain Cluster-Central CCCs, Core–Delta structures, structural DNA, probability-based dispatch information, provenance, local rules, ANN or LLM specialists, user plugins, and other Per-Node Intelligence.

The framework is intentionally domain-general. It does not require one metric, one tree topology, one sequence length, or one intelligence technology. Instead, it defines a reusable structural interface through which domain-specific individuals can become organized, searchable, localizable, and incrementally extensible structural knowledge.

---

# 1. From a Population to a Structure

Many intelligent systems begin with a population:

$$
\mathcal{X}=
\{x_1,x_2,\ldots,x_N\}
$$

The individuals may be:

* time-series segments,
* market trajectories,
* biological observations,
* molecules,
* genes,
* patient-independent research records,
* behavioral sequences,
* CallingGraphs,
* program traces,
* machine states,
* sensor trajectories,
* plans,
* decisions,
* or other structurally representable objects.

A conventional system may store these individuals independently.

Structural Folding asks a different question:

> **What reusable structure exists across the population?**

Instead of treating every individual as an isolated object, the system attempts to discover:

* shared structure,
* recurring neighborhoods,
* central patterns,
* structural differences,
* reusable dispatch rules,
* stable local regularities,
* and meaningful exceptions.

The target is therefore not simply:

```text id="4e7r2m"
Many Individuals
      ↓
Compressed Individuals
```

but:

```text id="d8cq1n"
Many Individuals
      ↓
Comparable Structural Representations
      ↓
Shared Structure + Localized Difference
      ↓
Reusable Structural Memory
```

This distinction is fundamental.

---

# 2. Structural Folding Is More Than Compression

Compression attempts to reduce representation cost.

Structural Folding has a stronger objective.

It attempts to preserve what future intelligence needs.

A useful Fold may therefore preserve:

```text id="a5p0g3"
Core
Delta
Neighborhood
Probability
Dispatch
Context
Provenance
Outcome
Local Intelligence
Counter-Evidence
```

A Fold can even consume more metadata than a naive compressed representation if that metadata significantly improves:

* localization,
* reasoning,
* search,
* validation,
* generation,
* or continual learning.

Thus:

> **Structural Folding is intelligence-oriented structural compression, not compression for its own sake.**

Its success should ultimately be judged by the usefulness of the resulting structural memory.

---

# 3. The Three General Mechanisms

Generic Structural Folding can be organized around three general mechanisms:

```text id="4k0jv7"
I. Generic Structural Representation
              ↓
II. Generic Structural Folding
              ↓
III. Generic Per-Node Intelligence
              ↓
       Structural Memory
```

These mechanisms separate domain-specific representation from domain-general structural operations.

They also allow the framework to evolve without requiring every domain to use the same data model or specialist intelligence.

---

![Fig-002 — Three General Mechanisms of Structural Folding](../figures/Fig-002-Three-General-Mechanisms-of-Structural-Folding.png)

*Fig-002 — Three General Mechanisms of Structural Folding. Generic Structural Representation creates comparable individuals, Generic Structural Folding extracts reusable shared structure and localized difference, and Generic Per-Node Intelligence attaches specialized intelligence to structural locations.*

---

# 4. General Mechanism I — Generic Structural Representation

## 4.1 GenericContainerStarmap

The canonical representation boundary in GFSFUI is the:

> **GenericContainerStarmap**

Conceptually:

$$
x_i
\rightarrow
S_i
$$

where \(x_i\) is a raw or domain-specific individual and \(S_i\) is its structurally operable representation.

A GenericContainerStarmap may contain:

```text id="m4dd76"
Individual
│
├── Scalar Properties
├── Categorical Properties
├── Sequence Properties
├── Temporal Properties
├── Structural Roles
├── Relations
├── Bigram / Trigram Features
├── Context
├── Outcome
└── Domain-Specific Elements
```

The representation does not require every individual to contain every possible field.

It provides a general container within which structurally meaningful elements can be exposed.

---

# 5. The Structuralization Boundary

The transformation:

```text id="n42azp"
Raw Domain Object
        ↓
GenericContainerStarmap
```

creates a major architectural boundary.

Above the boundary lies domain-specific interpretation.

Below the boundary lies reusable Structural Intelligence machinery.

```text id="4j3d8s"
DOMAIN-SPECIFIC WORLD
────────────────────────────
Segmentation
Feature Selection
Domain Semantics
Context Extraction
Role Identification
Graph Extraction
        ↓
GenericContainerStarmap
════════════════════════════
STRUCTURALIZATION BOUNDARY
════════════════════════════
        ↓
Metric Comparison
Differential Structure
CCC
DNA
Dispatch
Per-Node Intelligence
Structural Search
────────────────────────────
DOMAIN-GENERAL SI CORE
```

This allows the same Folding machinery to operate over very different domains.

A central principle follows:

> **Domain-specific representation at the edge; domain-independent structural intelligence in the core.**

---

# 6. Policy-Guided Structuralization

The Starmap should not be assumed to appear automatically.

A domain may require a structuralization policy.

For example:

```text id="i2gn8h"
Raw Sequence
    ↓
Segmentation Policy
    ↓
Selected Window
    ↓
Feature Policy
    ↓
GenericContainerStarmap
```

or:

```text id="c1j64e"
Program
   ↓
CallingGraph Extraction
   ↓
Node / Edge / Path Selection
   ↓
Bigram / Trigram Extraction
   ↓
GenericContainerStarmap
```

The policy determines what the Folding system is allowed to see.

A poor structuralization policy can hide useful structure.

A better policy can expose it.

Therefore structuralization itself becomes a legitimate target of intelligence.

---

# 7. Representation Policies Can Compete

GFSFUI does not require one representation policy to be selected permanently.

Multiple candidate structuralizations can be evaluated:

```text id="h24g78"
                 Raw Population
                       │
          ┌────────────┼────────────┐
          ↓            ↓            ↓
       Policy A     Policy B     Policy C
          ↓            ↓            ↓
       Starmap A    Starmap B    Starmap C
          ↓            ↓            ↓
        Fold A       Fold B       Fold C
          └────────────┼────────────┘
                       ↓
             Comparative Validation
```

The system can therefore search for better ways to represent the problem.

This produces a higher-level learning process:

> **Intelligence can search not only within a structure, but also for the structure in which future intelligence should operate.**

---

# 8. General Mechanism II — Metric and Structural Comparison

Once individuals have comparable representations, Structural Folding requires a mechanism for comparing them.

Let:

$$
d(S_i,S_j)
$$

denote a metric or structural comparison between Starmaps \(S_i\) and \(S_j\).

The function need not be Euclidean distance.

Possible comparisons include:

* Euclidean distance,
* Manhattan distance,
* cosine similarity,
* weighted sequence distance,
* domain-specific distance,
* graph similarity,
* Bigram overlap,
* Trigram overlap,
* role similarity,
* DNA similarity,
* outcome-conditioned similarity,
* or composite metrics.

The important requirement is:

> **The comparison must expose useful structural neighborhoods or differences.**

---

# 9. Metric Is a Localization Operator

A metric does not need to solve the final intelligence problem.

Its first responsibility may simply be to answer:

> **Where should this individual be examined?**

This changes the role of metric comparison.

Instead of:

```text id="24k8vx"
Metric
  ↓
Final Answer
```

GFSFUI often uses:

```text id="n8dzz3"
Metric
  ↓
Structural Neighborhood
  ↓
Relevant Node
  ↓
Local Intelligence
  ↓
Final Analysis
```

This is a much weaker requirement on the metric and a much stronger architecture for the system.

A moderately useful metric may still provide substantial value if it reliably reduces the search space.

Thus:

> **Metric similarity is primarily a structural localization mechanism, not necessarily a complete intelligence mechanism.**

---

# 10. From Similarity to Structural Neighborhoods

Suppose multiple individuals are structurally close:

$$
S_1,S_2,\ldots,S_k
$$

The system may construct a local neighborhood:

$$
\mathcal{N}=
\{S_1,S_2,\ldots,S_k\}
$$

The neighborhood becomes a candidate unit of Folding.

Within it, the system can ask:

* What is shared?
* What varies?
* Which properties are stable?
* Which properties correlate with outcomes?
* Which structural differences matter?
* Can a central structural representation be constructed?
* Can future individuals be dispatched here?

This is the transition from similarity computation to Structural Folding.

---

# 11. Cluster-Central CCC

A central construct is the:

> **Cluster-Central CCC**

The Cluster-Central CCC represents the reusable structural center of a neighborhood.

Conceptually:

$$
CCC(\mathcal{N})=
\text{StructuralCenter}
(
S_1,\ldots,S_k
)
$$

The exact implementation is domain-dependent.

It may include:

* central values,
* probability distributions,
* representative sequences,
* structural features,
* dispatch probabilities,
* outcome distributions,
* trigger information,
* DNA summaries,
* confidence information,
* and provenance references.

The Cluster-Central CCC is therefore more than a centroid.

---

# 12. CCC as a Structural Joint

The CCC connects several parts of the architecture.

```text id="czt95j"
Representation
     ↓
Similarity
     ↓
Neighborhood
     ↓
    CCC
 ┌────┼─────┬─────┐
 ↓    ↓     ↓     ↓
Memory Probability Dispatch Validation
```

It may function simultaneously as:

1. **Representation** — what is structurally central here?
2. **Probability** — how are properties or outcomes distributed?
3. **Dispatch** — does a new individual belong here?
4. **Runtime Routing** — which next structural region should be examined?
5. **Validation Reference** — how does a new observation differ from the existing Fold?

This makes the CCC a structural joint between learning and runtime intelligence.

---

# 13. Metric Differential Structure

Repeated neighborhood formation and CCC construction can produce a hierarchical structural organization.

A canonical form is the:

> **Metric Differential Tree**

```text id="ozj83r"
                   Root CCC
                      │
          ┌───────────┼───────────┐
          ↓           ↓           ↓
        CCC-A       CCC-B       CCC-C
          │                       │
      ┌───┴───┐               ┌───┴───┐
      ↓       ↓               ↓       ↓
    A1       A2              C1       C2
```

Each level reduces structural uncertainty.

Each branch represents a meaningful difference.

Each node can become a structural address.

---

# 14. The Tree Is Not the Fundamental Object

Although a tree is a particularly useful runtime embodiment, the deeper concept is:

> **Metric Differential Structure**

The canonical transformation is:

$$
\text{Similarity}
\rightarrow
\text{Shared Structure}
\rightarrow
\text{Difference Localization}
\rightarrow
\text{Dispatch}
$$

The structure could eventually take forms such as:

* a tree,
* a forest,
* multiple perspective trees,
* a structural network,
* a DAG,
* or a hybrid hierarchy.

Therefore GFSFUI does not define Structural Folding as “building a tree.”

The tree is one highly useful implementation of a more general principle.

---

# 15. Core and Delta

Structural Folding should preserve both commonality and difference.

Suppose a neighborhood contains a stable shared structure:

$$
C
$$

and individual or subgroup differences:

$$
\Delta_1,\Delta_2,\ldots,\Delta_m
$$

Then:

$$
S_i
\approx
C + \Delta_i
$$

This motivates the representation:

> **Core ± Delta**

The Core captures reusable common structure.

The Delta captures meaningful deviation.

```text id="h14g7f"
              CORE
                │
      ┌─────────┼─────────┐
      ↓         ↓         ↓
   Delta A   Delta B   Delta C
      ↓         ↓         ↓
 Outcome A  Outcome B  Outcome C
```

A useful Fold should not destroy Delta merely because Core is easier to compress.

Difference is often where future intelligence lives.

---

# 16. Difference Localization

One of the strongest consequences of Metric Differential Folding is that a difference obtains an address.

Instead of saying:

> This individual is unusual.

the system can say:

```text id="rd6iyq"
Domain
  ↓
Metric Perspective
  ↓
Tree
  ↓
Subtree
  ↓
Node
  ↓
CCC
  ↓
Specific Delta
```

This is **Difference Localization**.

It converts global ambiguity into local structural work.

That local work may include:

* validation,
* new rules,
* DNA discovery,
* ANN training,
* LLM reasoning,
* human review,
* branch formation,
* or a new Brain Unit.

---

# 17. Equal-Length Sequence Folding

Equal-length sequences provide a particularly clean canonical case.

Let:

$$
X=(x_1,x_2,\ldots,x_L)
$$

and a cluster center:

$$
C=(c_1,c_2,\ldots,c_L)
$$

A simple squared Euclidean comparison is:

$$
d^2(X,C)=
\sum_{i=1}^{L}(x_i-c_i)^2
$$

For dispatch purposes, the square root is often unnecessary because relative ordering is preserved.

This form has several engineering advantages:

* simple element-wise computation,
* fixed memory layout,
* vectorization,
* SIMD compatibility,
* GPU compatibility,
* batching,
* predictable cache behavior,
* and straightforward centroid computation.

This is one reason equal-length sequences are useful for canonical demonstrations.

---

# 18. Equal Length Is Not a Theoretical Requirement

GFSFUI does not require every individual to have equal length.

Variable-length structures may be handled through:

* alignment,
* sequence merging,
* n-gram representations,
* path decomposition,
* structural normalization,
* graph comparison,
* hierarchical matching,
* or other domain-specific methods.

The tradeoff is computational.

A useful engineering principle is therefore:

> **Use the simplest structurally adequate comparison first; escalate only when the problem requires it.**

For CallingGraphs, for example, fixed-order Bigram and Trigram representations may provide an inexpensive first structural comparison before whole-path or graph-level matching is attempted.

---

# 19. Multiple Metrics and Multiple Perspectives

One representation may support multiple meaningful notions of similarity.

For example:

```text id="9z3ch2"
                 Individual
                     │
        ┌────────────┼────────────┐
        ↓            ↓            ↓
   Metric A      Metric B      Metric C
        ↓            ↓            ↓
     Tree A        Tree B        Tree C
```

These may represent:

* different domains,
* different time scales,
* different feature subsets,
* different structural roles,
* different sequence granularities,
* or different reasoning perspectives.

A system may therefore maintain multiple Metric Differential structures over the same population.

This supports:

> **Per-Metric Perspective Intelligence**

A new individual can be evaluated through more than one structural coordinate system.

---

# 20. Cross-Perspective Agreement and Disagreement

Multiple metric perspectives create additional intelligence.

Suppose:

```text id="1lmh7v"
Metric A → Node X
Metric B → Node X
Metric C → Node X
```

The agreement strengthens localization.

But suppose:

```text id="t4k0sq"
Metric A → Node X
Metric B → Node X
Metric C → Node Y
```

The disagreement is itself information.

It may indicate:

* a boundary case,
* a hidden Delta,
* a missing feature,
* a context dependency,
* a new subgroup,
* or a poor metric.

Thus multi-metric Folding does more than improve accuracy.

It creates a mechanism for discovering structural tension.

---

# 21. General Mechanism III — Per-Node Intelligence

Once a Metric Differential structure exists, each node becomes a potential intelligence address.

A node may contain:

```text id="vdw1k3"
Node
│
├── Cluster-Central CCC
├── Probability Table
├── DNA CCC
├── Rules
├── ANN
├── LLM Specialist
├── Domain Algorithm
├── User Plugin
├── Search Policy
├── Validation Policy
└── Provenance
```

This is:

> **Per-Node Intelligence**

The system no longer requires every query to invoke the same global model.

---

# 22. Intelligence Addressing

The structural hierarchy provides a route:

```text id="qf32v5"
Query
  ↓
Representation
  ↓
Metric Perspective
  ↓
Tree
  ↓
Node
  ↓
Local Specialist
```

This is analogous to assigning intelligence a structural address.

The address may be:

$$
A =
(Domain,
Metric,
Tree,
Node,
CCC,
Context)
$$

The exact schema may evolve, but the principle is important:

> **Learning and reasoning can occur at a known structural location.**

This makes local growth possible.

---

# 23. Per-Node Intelligence Is Open

GFSFUI does not prescribe one node model.

A node may use:

### Lightweight intelligence

* lookup,
* probability,
* CCC,
* DNA,
* threshold,
* rules.

### Medium intelligence

* regression,
* small neural network,
* domain-specific model,
* graph algorithm.

### Heavy intelligence

* large ANN,
* LLM,
* agent,
* external reasoning system.

### Human or external intelligence

* user plugin,
* expert review,
* external service,
* certified domain tool.

Thus:

> **Per-Node Intelligence is an architectural slot, not a fixed algorithm.**

---

# 24. Compute-by-Need

Per-Node Intelligence enables a natural escalation policy.

```text id="0pk0h2"
Index / Cache
     ↓
Metric Dispatch
     ↓
CCC
     ↓
DNA / Rules
     ↓
Small Specialist
     ↓
Large Specialist
     ↓
LLM / External Tool
```

A query that can be resolved at the CCC level should not automatically invoke an expensive global model.

This leads to:

> **Do not invoke expensive intelligence when structural dispatch already resolves the case.**

The architecture therefore separates:

* structural memory size,
* active computation,
* and specialist complexity.

---

# 25. Structural DNA

Metric similarity is not the only possible structural relation.

A node may contain combinations of features that act as structural DNA.

A general extraction process is:

```text id="odn5yi"
GenericContainerStarmap
        ↓
Element Selection Policy
        ↓
Typed / Named Elements
        ↓
Candidate DNA
        ↓
Observed Dispatch / Trigger
        ↓
DNA CCC
```

DNA can contain:

* individual attributes,
* feature combinations,
* sequence fragments,
* Bigram relations,
* Trigram relations,
* structural roles,
* contextual conditions,
* or domain-specific elements.

This gives the system another way to organize local knowledge.

---

# 26. DNA as a Second Structural Coordinate

An important case occurs when two individuals are distant under the primary metric but share a meaningful DNA structure.

```text id="z3p4wg"
Individual A ── Metric ── distant ── Individual B
      │                               │
      └──────── DNA similar ──────────┘
```

This can reveal structural equivalence that the primary metric missed.

Conversely:

```text id="i3a7ov"
Individual A ── Metric ── near ── Individual B
      │                             │
      └──────── DNA different ──────┘
```

may expose an important hidden difference.

Metric and DNA can therefore function as complementary structural coordinates.

---

# 27. Two-Way DNA CCC

Suppose DNA \(D\) is associated with outcome \(Y\).

A one-way observation is:

$$
D \rightarrow Y
$$

A stronger structural test also examines:

$$
Y \rightarrow D
$$

This is the basic idea of **Two-Way DNA CCC**.

It asks:

* When \(D\) occurs, how often does \(Y\) occur?
* When \(Y\) occurs, how often is \(D\) present?

The objective is not to establish causality automatically.

The objective is to expose asymmetry, missing conditions, weak patterns, and structural alternatives.

This makes Two-Way DNA CCC useful for:

* dispatch,
* triggering,
* validation,
* structural consistency,
* and Delta discovery.

---

# 28. Two-Way CCC Is Not Limited to Leaves

A simplified implementation may attach DNA CCCs only to leaf nodes.

The general framework does not impose this restriction.

Any meaningful node may support local CCC or DNA intelligence:

```text id="blqlaz"
Root
 │
 ├── Intermediate Node
 │      ├── CCC
 │      ├── DNA
 │      └── Specialist
 │
 └── Leaf
        ├── CCC
        ├── DNA
        └── Specialist
```

This supports multiple analysis granularities.

A high-level node may capture broad regularities.

A lower-level node may capture specialized conditions.

The best intelligence location is therefore an empirical question rather than a fixed architectural rule.

---

# 29. Structural Memory

After Folding, the system does not merely retain a tree.

Its structural memory may contain several layers:

```text id="psnjw4"
STRUCTURAL MEMORY
│
├── Individual References
├── GenericContainerStarmaps
├── Metric Structures
├── Differential Trees / Networks
├── Cluster-Central CCCs
├── Core Structures
├── Delta
├── DNA
├── Dispatch Tables
├── Triggers
├── Outcomes
├── Per-Node Specialists
├── Evidence
├── Counter-Evidence
├── Context
└── Provenance
```

Structural memory is therefore a **multi-layer intelligence substrate**.

---

# 30. Memory Does Not Require Everything to Stay Hot

Large systems may separate memory into tiers.

```text id="g82mqn"
HOT
│
├── Tree Topology
├── CCC
├── Frequent DNA
├── Dispatch
└── Active Node Intelligence

WARM
│
├── Detailed Starmaps
├── Less-Frequent Delta
├── Historical Outcomes
└── Local Evidence

COLD
│
├── Raw Individuals
├── Full Historical Sequences
├── Archived Evidence
└── Deep Provenance
```

This allows:

> **Global structural memory with a small active intelligence footprint.**

The system can preserve large amounts of experience without activating all of it for every query.

---

# 31. Structural Folding Ratio

One useful future measurement is the amount of memory required after Folding relative to raw experience.

Define:

$$
\rho_f =
\frac{M_{\text{folded}}}
     {M_{\text{raw}}}
$$

where:

* \(M_{\text{raw}}\) is raw memory,
* \(M_{\text{folded}}\) is retained structural memory.

A corresponding gain is:

$$
G_f =
\frac{M_{\text{raw}}}
     {M_{\text{folded}}}
$$

These metrics should be interpreted carefully.

A low \(\rho_f\) is not automatically better if important Delta, context, or provenance has been destroyed.

The objective is not maximum compression.

It is:

> **maximum reusable structural intelligence per retained unit of memory.**

---

# 32. Folding Cost and Runtime Cost Are Different

A critical distinction is:

$$
C_{\text{system}}=
C_{\text{fold/update}}
+
C_{\text{online}}
$$

Cluster-Central CCCs should normally be constructed or updated during Folding.

A runtime query should not recompute an entire cluster center from all historical members unless explicitly required.

Instead:

```text id="0ic40y"
New Individual
      ↓
Representation
      ↓
Compare with Existing CCCs
      ↓
Structural Dispatch
```

This separation is essential for scalable runtime behavior.

---

# 33. Canonical Online Metric Cost

For a simple tree-routing system with:

* tree depth \(D\),
* average candidate CCC count \(B\),
* representation length \(L\),

the metric-comparison component can often be organized approximately as:

$$
C_{\text{metric}}=
O(D \cdot B \cdot L)
$$

before optional local specialists are invoked.

This is not a benchmark claim.

It illustrates the architectural objective:

> **Online computation should scale primarily with the activated structural path rather than the total population whenever the Folding structure permits it.**

---

# 34. Structural Growth

Structural memory should not be static.

A new individual can be dispatched to a node and compared with existing local structure.

```text id="dphf9y"
New Individual
      ↓
Node Dispatch
      ↓
Compare with CCC / DNA
      ↓
 ┌────┴────┐
 ↓         ↓
Match    Difference
 ↓         ↓
Update    Delta
           ↓
       Validation
           ↓
         Branch
```

This produces local structural growth.

---

# 35. From Delta to Brain Unit

Repeated meaningful Delta may justify increasingly specialized intelligence.

A useful progression is:

```text id="k2yg3x"
Observation Difference
        ↓
Candidate Delta
        ↓
Persistent Delta
        ↓
Sub-CCC
        ↓
Branch
        ↓
Specialized Intelligence
        ↓
Brain Unit
```

Thus a Brain Unit does not need to be arbitrarily preallocated.

It can emerge because persistent local difference justifies specialization.

This gives a structural interpretation:

> **A Brain Unit is a structurally justified specialization created by persistent localized difference.**

---

# 36. Low-Blast-Radius Learning

Global parameter updating can affect behavior across a large model.

Localized Structural Folding offers another possibility.

If new evidence belongs to one structural region:

$$
\Delta S_{\text{system}}
\approx
\Delta S_{\text{local}}
$$

rather than requiring:

$$
\Delta S_{\text{system}}
\approx
\Delta S_{\text{global}}
$$

This is not always possible.

Some discoveries genuinely require global restructuring.

But when localization succeeds, the system gains:

* smaller update scope,
* clearer causality of change,
* easier A/B testing,
* easier rollback,
* easier certification,
* and reduced unintended impact.

This property can be described as:

> **Low-Blast-Radius Learning**

---

# 37. Structural Folding and Continual Learning

Continual learning can therefore be expressed as:

```text id="bh30f7"
Observe
   ↓
Dispatch
   ↓
Compare
   ↓
Reinforce or Extract Delta
   ↓
Validate
   ↓
Grow Local Structure
   ↓
Continue
```

The system does not merely accumulate samples.

It accumulates and refines structure.

Thus:

> **Continual Structural Learning = Continual Structural Folding + Localized Structural Growth**

This creates a natural bridge between GFSFUI and Brain-Unit / Structural Continual Learning research.

---

# 38. Structural Folding Is Not Restricted to Large Data

Large populations make structural regularities easier to estimate, but Folding can begin earlier.

A small number of high-information examples may form:

* a candidate neighborhood,
* a candidate CCC,
* a candidate DNA,
* or a candidate structural hypothesis.

The Fold can then be tested through additional evidence.

This leads to an important distinction:

> **Initiating a Fold is not the same as certifying a Fold.**

Sparse evidence may be enough for the former.

Stronger evidence is generally required for the latter.

This is the basis for later GFSFUI work on 3-Cat Learning, counter-evidence search, and sparse-data Structural Intelligence.

---

# 39. CallingGraph as a Foldable Population

CallingGraphs illustrate the generality of the framework.

A CallingGraph is not structurally privileged.

It is another type of individual.

Given a population:

$$
CG_1,CG_2,\ldots,CG_N
$$

each CallingGraph can be converted into a GenericContainerStarmap.

Possible elements include:

```text id="8f7f63"
CallingGraph
│
├── Node Roles
├── Edge Types
├── Path Features
├── Bigrams
├── Trigrams
├── Entry / Exit Structure
├── Failure Paths
├── Context
└── Outcome / Certification
```

The population can then use the same machinery:

```text id="uj5asf"
CallingGraphs
     ↓
GenericContainerStarmap
     ↓
Metric / Structural Similarity
     ↓
Metric Differential Structure
     ↓
CG CCC / DNA / Core ± Delta
     ↓
Per-Node Intelligence
```

This is a major architectural simplification.

> **CallingGraph does not require a separate Structural Folding theory.**

It requires a domain adapter into the general Folding framework.

---

# 40. Thin Domain Plugins

A domain should ideally contribute only what is structurally specific to that domain.

For CallingGraphs:

```text id="xftwqw"
CG Domain Adapter
│
├── CG Extraction
├── CG Segmentation
├── Starmap Builder
├── Similarity Plugin
├── Bigram / Trigram Extractor
├── DNA Plugin
└── Certification Plugin
```

The reusable core remains:

```text id="jkv9b0"
Metric Differential Structure
CCC
Core ± Delta
Per-Node Intelligence
Two-Way Search
Structural Growth
```

This supports a strong engineering rule:

> **Keep domain intelligence at the edge when the core mechanism can remain general.**

---

# 41. Generic Structural Folding Pipeline

The complete canonical Folding pipeline is:

```text id="l6lscu"
RAW INDIVIDUAL POPULATION
          │
          ▼
POLICY-GUIDED STRUCTURALIZATION
          │
          ▼
GENERICCONTAINERSTARMAP
          │
          ▼
METRIC / STRUCTURAL COMPARISON
          │
          ▼
SIMILARITY NEIGHBORHOODS
          │
          ▼
CLUSTER-CENTRAL CCC
          │
          ▼
METRIC DIFFERENTIAL STRUCTURE
          │
     ┌────┼────┐
     ▼    ▼    ▼
   CORE  DELTA DNA
     │    │    │
     └────┼────┘
          ▼
PER-NODE INTELLIGENCE
          │
          ▼
STRUCTURAL MEMORY
```

This pipeline can be summarized as:

> **Represent → Compare → Cluster → Centralize → Differentiate → Dispatch → Specialize → Remember**

---

# 42. Two Architectural Properties

The three general mechanisms are supported by two architectural properties.

---

## 42.1 Open Intelligence Integration

The Folding structure can integrate:

* CCC,
* DNA,
* rules,
* ANN,
* LLM,
* domain algorithms,
* search,
* plugins,
* tools,
* and human review.

No one intelligence mechanism is required to dominate every node.

---

## 42.2 End-to-End Structural Traceability

Every important structural object should remain traceable.

```text id="1j0fvl"
Decision / Prediction
       ↓
Node Intelligence
       ↓
CCC / DNA
       ↓
Tree Node
       ↓
Metric Perspective
       ↓
GenericContainerStarmap
       ↓
Original Individual
```

This allows the system to answer:

* Why was this node selected?
* Which CCC supported the dispatch?
* Which DNA triggered the outcome?
* Which individuals formed the CCC?
* Which evidence contradicts it?
* Which source produced the original individual?

Traceability is therefore part of the architecture, not an afterthought.

---

# 43. The Structural Folding Machine

The central theoretical abstraction of this paper can now be stated.

A Generic Structural Folding Machine performs:

$$
\boxed{
\text{Individual Population}
\rightarrow
\text{Shared Structure}
+
\text{Localized Difference}
+
\text{Structural Addresses}
+
\text{Reusable Intelligence}
}
$$

Its fundamental operation is:

$$
\boxed{
\text{Similarity}
\rightarrow
\text{Shared Structure}
\rightarrow
\text{Difference Localization}
\rightarrow
\text{Dispatch}
}
$$

Its runtime consequence is:

$$
\boxed{
\text{Global Structural Memory}
+
\text{Local Intelligence Activation}
}
$$

Its learning consequence is:

$$
\boxed{
\text{Persistent Delta}
\rightarrow
\text{Local Structural Growth}
}
$$

---

# 44. What Generic Structural Folding Does Not Require

The framework does not require:

* one universal metric;
* one universal representation policy;
* one fixed sequence length;
* one tree;
* one depth;
* one cluster algorithm;
* one CCC implementation;
* one DNA encoding;
* one node intelligence model;
* one global neural network;
* one universal naming system;
* or one domain.

These are implementation choices.

The General Framework requires something more basic:

> **Individuals must become structurally comparable, repeated structure must become reusable, meaningful difference must remain localizable, and intelligence must be able to act on the resulting structural addresses.**

---

# 45. Canonical Principles of Generic Structural Folding

### Principle 1 — Structuralize Before Folding

Raw domain objects should be transformed into structurally operable representations.

### Principle 2 — Compare for Localization

Metric comparison need not solve the final problem; it must help find the relevant structural neighborhood.

### Principle 3 — Fold Shared Structure

Repeated structure should become reusable CCC, Core, DNA, or related memory.

### Principle 4 — Preserve Delta

Meaningful differences must not disappear inside an average.

### Principle 5 — Give Difference an Address

Structural hierarchy should localize where a difference occurs.

### Principle 6 — Attach Intelligence Locally

Nodes should be able to host the intelligence appropriate to their structural region.

### Principle 7 — Allow Multiple Perspectives

Different metrics and granularities may reveal different valid structures.

### Principle 8 — Escalate Compute by Need

Expensive intelligence should follow structural localization where possible.

### Principle 9 — Preserve Provenance

Folded knowledge must remain traceable to its supporting individuals and context.

### Principle 10 — Let Persistent Difference Grow Structure

Repeated Delta should be able to create new CCCs, branches, specialists, and Brain Units.

---

# 46. From Structural Folding to Structural Search

Once Folding has created:

```text id="y60a2c"
Tree
CCC
Core
Delta
DNA
Node Intelligence
Context
Provenance
```

the next question is no longer:

> How do we build structural memory?

It becomes:

> **How do we search that structural memory—especially for supporting evidence, counter-evidence, alternative structures, and growth opportunities?**

This is the transition from Generic Structural Folding to the **Structural Search Plane**.

That subject is developed in:

> **GFSFUI-003 — Structural Search, Counter-Evidence, and Continual Structural Growth**

---

# 47. Final Perspective

Generic Structural Folding transforms a population into something qualitatively different from a database of independent individuals.

It creates:

* reusable shared structure,
* localized difference,
* structural addresses,
* probability-based CCCs,
* searchable DNA,
* multiple metric perspectives,
* Per-Node Intelligence,
* context-preserving provenance,
* and explicit locations for future growth.

The central transition is:

```text id="3s7ccu"
INDIVIDUALS
     ↓
REPRESENT
     ↓
COMPARE
     ↓
FOLD
     ↓
CORE + DELTA
     ↓
LOCALIZE
     ↓
DISPATCH
     ↓
SPECIALIZE
     ↓
STRUCTURAL MEMORY
```

The resulting memory is not the endpoint.

It is the substrate on which Structural Search, Structural Falsification, Continual Growth, and Structural Unfolding can operate.

---

## Canonical Summary

> **GenericContainerStarmap provides the structuralization boundary.**

> **Metric and structural comparison provide localization.**

> **Cluster-Central CCC converts neighborhoods into reusable structural centers and dispatch structures.**

> **Metric Differential structures organize shared structure and localized difference.**

> **Core preserves common structure; Delta preserves meaningful variation.**

> **Per-Node Intelligence turns structural nodes into intelligence addresses.**

> **Structural DNA provides a complementary coordinate beyond primary metric similarity.**

> **Multiple metrics provide multiple structural perspectives.**

> **Persistent local Delta provides a path toward branches, specialists, and Brain Units.**

> **Structural Memory preserves not only what is similar, but also where and how intelligence should act.**

Therefore:

> **Represent → Compare → Fold → Differentiate → Dispatch → Specialize → Remember.**

---

**GFSFUI-002**
**Generic Structural Folding: From Individuals to Structural Memory**
