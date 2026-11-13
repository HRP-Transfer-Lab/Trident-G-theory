# Trident-G: A Coupled-Dynamical Theory of Homeostatic General Intelligence

Version 0.2 — Plain-English interpretation and mathematical appendix

## Overview

The proposed Trident-G model describes general intelligence as a **self-regulating, adaptive system that coordinates flexible cognition, consolidated knowledge and interactions with changing environments (niches).**

Its central hypothesis is that intelligence depends not simply on possessing cognitive resources, but on regulating how those resources are deployed to explore possibilities, discover relational structures, solve problems, consolidate knowledge and expand future capabilities.

The mathematical framework combines five interacting mechanisms\:

1. **Homeostatic regulation\:** Maintaining effective cognition within viable operating conditions.
2. **Near-critical fluid cognition (Gf)\:** Coordinating generative and relational processes across four Trident computational branches.
3. **Crystallised intelligence (Gc)\:** Stabilising and reusing acquired knowledge, strategies and relational invariants.
4. **Recursive learning\:** Using Gf to generate knowledge that becomes Gc, which subsequently supports further Gf reasoning.
5. **Coupled niche dynamics\:** Adapting to environments while also modifying them through intelligent action.

A distinctive hypothesis is that Gc-dominated processing preferentially operates in relatively stable, slightly subcritical regimes, whereas Gf recruits flexible near-critical dynamics, potentially involving brief supercritical excursions.

This is a proposed mechanistic distinction, not yet an established neuroscientific result. The criticality of neural activity and the stability of knowledge representations must be measured independently.

---

# Part I. Plain-English interpretation of the equations

## 1\. The adaptive control equation: the cusp

\[
\boxed{
dx_t=
[-4x_t^3+2\xi_t x_t+\delta_t]dt
+\sigma_xdW_t
}
\]

**What this means\:** Intelligence continually adjusts between different modes of adaptive cognition, rather than operating in one fixed mode.

The variable \(x_t\) represents the system's current adaptive mode. We provisionally define negative values as favouring exploitation of established solutions and positive values as favouring exploration of alternatives.

Two control parameters govern the dynamics.

- \(\xi_t\) determines whether the system can support alternative stable adaptive modes.
- \(\delta_t\) biases the system towards one mode or the other.

The final term introduces random fluctuations, allowing for spontaneous variation in cognitive state.

### Why a cusp?

The cusp allows a system to exhibit both gradual adjustment and sudden transitions.

A small change in task demands might produce little observable change until a critical threshold is crossed. At that point, the system may abruptly abandon an established strategy and begin exploring a new one.

It can also exhibit *hysteresis*\: the threshold for moving into exploration need not be identical to the threshold for returning to exploitation.

**Trident-G interpretation\:** Effective intelligence involves regulating not only how much exploration occurs, but also when the system should persist, switch strategies or reorganise its approach.

The cusp is the model's organising control mechanism; it is not itself a direct measure of neural criticality.

## 2\. Effective capacity and homeostatic regulation

\[
\boxed{
\xi_t=
g(\mathbf c_t,\eta_t,\chi_t,\mathbf h_t,
\mathbf k_t^{Gc},\mathbf b_t)-F_t^\star
}
\]

**What this means\:** The stability and flexibility of adaptive cognition depend on the resources available to the system relative to its defended operating requirements.

The function \(g\) combines several influences\:

| Variable | Psychological interpretation |
|--------|--------|
| \(\mathbf c_t\) | Available cognitive capacities |
| \(\eta_t\) | Meta-efficacy: estimated ability to regulate outcomes |
| \(\chi_t\) | Coherence between representations, goals and actions |
| \(\mathbf h_t\) | Regulatory resources and internal conditions |
| \(\mathbf k_t^{Gc}\) | Accessible crystallised knowledge |
| \(\mathbf b_t\) | Current activity of the four Gf computational branches |
| \(F_t^\star\) | Defended regulatory threshold or reference level |

The resulting \(\xi_t\) represents an effective regulatory margin, not a conventional IQ score.

A person may possess substantial cognitive capacity but be unable to deploy it effectively because of uncertainty, poor strategy selection, conflicting goals or excessive demands.

Conversely, strong domain knowledge and well-developed strategies may allow a person to operate effectively with lower immediate computational demands.

**Trident-G interpretation\:** Intelligence involves maintaining a workable relationship between cognitive demands, resources and regulatory control.

A larger \(\xi_t\) expands the mathematical region in which alternative stable modes can coexist. It should not automatically be interpreted as greater intelligence: the adaptive value depends on task demands and the system's ability to switch appropriately.

## 3\. Exploration–exploitation regulation across niches

\[
\boxed{
\delta_t=
u_t+
\sum_n\lambda_n
\psi_n(\mathbf z_{n,t},\mathbf k_{n,t})
+\boldsymbol\omega^\top\mathbf b_t
}
\]

**What this means\:** Whether a person explores or exploits depends on three interacting influences.

**Internally generated control (\(u_t\)\).** The individual may deliberately choose to experiment, persevere, change strategy or revisit an established solution.

**Environmental influences.** Each niche creates opportunities, demands and constraints. A rapidly changing professional environment may encourage exploration, while a familiar routine may favour exploitation.

**Current Gf processing.** The active computational branches influence which adaptive mode is most appropriate.

The coefficients \(\lambda_n\) describe the influence of each niche, while \(\boldsymbol\omega\) describes how branch activity contributes to the exploration–exploitation bias.

**Trident-G interpretation\:** Adaptive intelligence is not simply responding to uncertainty. It involves regulating the relationship between internally chosen goals, cognitive processing and opportunities in the environment.

This is where strategic autonomy enters the formal system.

## 4\. The four Gf computational branches

\[
\boxed{
d\mathbf b_t=
\mathbf F_b(
\mathbf b_t,\mathbf o_t,\mathbf k_t^{Gc},
\mathbf k_t,\mathbf z_t,\mathbf c_t,
\boldsymbol\epsilon_t^{Gf})dt
+\Sigma_b\,d\mathbf W_t^{(b)}
}
\]

**What this means\:** Fluid cognition involves the coordinated operation of four computational processes.

These arise from crossing two dimensions\:

- Entropy-related generation and exploration versus mutual-information-related discovery of predictive relationships.
- Internally maintained representations versus externally anchored cognitive operations.

Four proposed Gf computational branches

INTERNAL × MUTUAL INFORMATION

**Relational inference**

Construct and integrate abstract relationships, models and analogies

INTERNAL × ENTROPY

**Generative exploration**

Produce possibilities, hypotheses and counterfactual models

EXTERNAL × MUTUAL INFORMATION

**Evidence integration**

Discover predictive relationships, constraints and regularities

EXTERNAL × ENTROPY

**Environmental exploration**

Sample alternatives, manipulate conditions and test possibilities

The vector \(\mathbf b_t\) represents the current engagement of these four processes.

Their dynamics depend on available observations, previous knowledge, niche conditions, capacities and criticality parameters.

These are computational branches, not necessarily four anatomically separate neural systems. They also should not be equated one-for-one with the four functional Trident capacities, which can recruit multiple branches.

### Why entropy and mutual information?

Entropy represents uncertainty or the diversity of possible states. Mutual information represents how much knowing one variable reduces uncertainty about another.

The two are complementary, rather than opposites: a system can have substantial uncertainty while also containing strong informative relationships.

The proposed Gf mechanism would use generative processes to produce or sample alternatives and relational processes to discover which structures are informative.

**Trident-G interpretation\:** Higher fluid intelligence may involve more effective coordination between generating possibilities and identifying the relational structure that makes those possibilities useful.

## 5\. Regulating the Gf criticality regimes

\[
\boxed{
\dot{\epsilon}^{Gf}_{i,t}
=
-\kappa_i
\left(
\epsilon^{Gf}_{i,t}
-\epsilon^{Gf,\star}_{i,t}
\right)
}
\]

Here, \(\epsilon^{Gf}_{i,t}\) is the effective criticality parameter for branch \(i\), while \(\epsilon^{Gf,\star}_{i,t}\) is its task-dependent target.

**What this means\:** Gf processing is hypothesised to regulate the dynamical regime of its constituent processes according to task demands.

Within an idealised neural branching approximation, the regime parameter can be defined as\:

\[
\epsilon_i=m_i-1
\]

where \(m_i\) represents effective activity propagation.

- \(\epsilon_i<0\)\: subcritical.
- \(\epsilon_i=0\)\: critical.
- \(\epsilon_i>0\)\: supercritical.

Your hypothesis is that Gf branches operate near this boundary, potentially with positive excursions during demanding exploration or synthesis.

The parameter \(\kappa_i\) specifies how quickly the system returns towards its target regime.

This is a regulatory equation: it explicitly prevents us from treating supercriticality as a permanent desirable state.

**Trident-G interpretation\:** Effective Gf requires controlled access to flexible computational regimes, rather than indiscriminately maximising neural excitation, variability or exploration.

The target regime could depend on novelty, uncertainty, relational complexity and available regulatory resources.

Importantly, the branching approximation is only one possible operationalisation of criticality. Empirical neural systems may require different estimators.

## 6\. Gc stabilisation and efficient knowledge use

\[
\boxed{
\dot{\epsilon}^{Gc}_t
=
-\kappa_{Gc}
\left(
\epsilon^{Gc}_t-
\epsilon^{Gc,\star}
\right)
\qquad
\epsilon^{Gc,\star}<0
}
\]

**What this means\:** Gc-dominated processing is hypothesised to return towards a relatively stable, slightly subcritical operating regime.

The distinction is functional.

Gf must actively construct or reorganise representations to handle novelty.

Gc enables the retrieval and application of representations already acquired through previous learning.

The proposed advantages of Gc include reduced processing demands, lower interference, reliable retrieval and efficient application of learned structures.

For an equivalent task outcome, we might hypothesise\:

\[
\mathbb E[C_{\mathrm{Gc\ retrieval}}]
<
\mathbb E[C_{\mathrm{Gf\ synthesis}}]
\]

where \(C\) represents incremental processing or energetic cost.

This inequality is a **separate empirical hypothesis**, not something that follows automatically from subcritical neural dynamics.

It also applies conditionally: knowledge retrieval may be expensive, and learning or consolidation can require substantial metabolic resources.

**Trident-G interpretation\:** Gc provides relatively stable, reusable cognitive structure, reducing the need to repeatedly solve familiar problems from first principles.

The contrast is between modes of computation, not two wholly independent brain systems.

## 7\. Gf synthesis: constructing a useful representation

\[
\boxed{
\mathbf r_t^\star=
\mathcal S(
\mathbf b_t,
\mathbf k_t^{Gc},
\mathbf k_t,
\mathbf o_t,
\mathbf z_t)
}
\]

**What this means\:** Gf combines information from the four computational branches with existing knowledge to construct a useful representation of the current problem.

The operator \(\mathcal S\) represents synthesis.

Its output, \(\mathbf r_t^\star\), might be a causal model, a relational structure, a solution strategy, a hypothesis or an abstract analogy.

For example, consider a scientist investigating an unexpected experimental finding.

The entropy-related branches generate alternative explanations and possible experiments. The mutual-information-related branches identify relationships between variables and constraints imposed by the evidence.

Previously acquired knowledge provides theoretical frameworks and relevant research findings.

Gf synthesis coordinates these contributions into a candidate explanatory model.

**Trident-G interpretation\:** Gf is not simply the capacity to maintain or manipulate unfamiliar information. It is the capacity to construct and select useful relational structures from interacting generative, inferential and knowledge-based processes.

Higher Gf might permit more complex relational synthesis, more effective integration of evidence and more rapid identification of structures that generalise.

These would need to be distinguished experimentally.

## 8\. Invariant learning: discovering transferable structure

\[
\boxed{
\dot{\mathbf q}_t=
\mathcal M(
\mathbf q_t,\mathbf r_t^\star,
\mathbf o_t,\mathbf a_t,\mathbf z_t)
}
\]

**What this means\:** The system tests whether the relational structures discovered during Gf synthesis remain valid across changes in circumstances.

The variable \(\mathbf q_t\) represents developing candidate invariants.

An invariant is a relationship or property that remains unchanged under a specified set of transformations.

For example, a scientist might discover that the same causal relationship holds across different experimental contexts. An entrepreneur might recognise an equivalent bottleneck structure across otherwise different business processes.

An invariant-learning mechanism should distinguish superficial similarity from preserved relational structure.

We can define a candidate invariant representation \(r\) such that\:

\[
r(TX)\approx r(X)
\]

where \(T\) changes the surface characteristics of a problem while preserving the relevant relationship.

This condition alone is insufficient: the representation must also retain information needed for successful prediction or action, otherwise a trivial constant representation would qualify.

The model must therefore learn **useful invariants**, not merely representations that remain unchanged.

### The Gf prediction

Your proposal implies\:

\[
\boxed{
\text{Higher Gf}
\;\Rightarrow\;
\text{greater capacity for learning useful invariants}
}
\]

More specifically, people with higher Gf should, other things being equal, be better at discovering complex relational structures that generalise across unfamiliar contexts.

The relationship might be moderated by Gc, existing conceptual knowledge, feedback quality and the transformations being learned.

**Trident-G interpretation\:** A major contribution of Gf to general intelligence may be the discovery of relational invariants that can subsequently be applied in novel circumstances.

This would give us a concrete mechanism linking Gf to far transfer.

## 9\. Gf-to-Gc banking: consolidating successful invariants

\[
\boxed{
\dot{\mathbf k}^{Gc}_t=
\kappa_bv_t
\mathcal B(\mathbf q_t,\mathbf r_t^\star)
-
\Gamma_{Gc}(\mathbf k_t^{Gc})
}
\]

**What this means\:** The most useful relational structures discovered by Gf become part of the relatively stable Gc knowledge bank.

The function \(\mathcal B\) represents knowledge banking or consolidation.

The validation coefficient \(v_t\), bounded between zero and one, reflects the evidence that a candidate representation is reliable and generalisable.

The final term allows for forgetting, interference, revision or obsolescence.

This is particularly important because the model should not consolidate every successful solution indiscriminately. Some solutions are highly context-specific, while others reveal reusable structure.

Banking might involve several transformations\:

- A demanding reasoning operation becomes a learned strategy.
- A discovered relationship becomes a conceptual schema.
- A repeated problem-solving sequence becomes a more automatic procedure.
- A transferable invariant becomes available for future reasoning.

**Trident-G interpretation\:** Gf produces candidate structures, learning evaluates them, and Gc stabilises sufficiently useful structures for efficient future reuse.

The resulting Gc can then support new Gf synthesis.

This formalises the recursive cycle\:

\[
\boxed{
Gf\rightarrow Gc\rightarrow Gf
}
\]

The important feature is that later Gf operations begin with access to richer, more structured knowledge than earlier operations.

## 10\. Cross-niche knowledge transfer

\[
\boxed{
\begin{aligned}
\dot{\mathbf k}_{n,t}
={}&\mathcal L_n(\mathbf k_{n,t},\mathbf o_t,\mathbf a_t)\\
&+\tau_n\mathcal T_n(\mathbf k_t^{Gc})\\
&+\sum_{m\neq n}\tau_{mn}
\mathcal T_{mn}(\mathbf k_{m,t})
\end{aligned}
}
\]

**What this means\:** Knowledge acquired in one niche can influence learning and performance in other niches.

There are three sources of change.

The first is direct learning within the current niche.

The second is the application of previously consolidated Gc knowledge.

The third is transfer from other niches through mappings that identify relevant structural correspondences.

The coefficients \(\tau_n\) and \(\tau_{mn}\) describe the effectiveness of these transfer processes.

For example, someone might learn a constraint-removal strategy while solving a research problem, recognise an equivalent structure in business operations, and apply the strategy to improve an organisational process.

The mathematical mappings must preserve task-relevant structure. The model should not assume that all knowledge transfers successfully.

**Trident-G interpretation\:** Far transfer depends on recognising and applying useful relational structure across differences in context.

It is not enough to improve performance on the original learning task. General intelligence should involve a demonstrated capacity to reuse what has been learned under meaningfully transformed conditions.

## 11\. Development of the four Trident capacities

\[
\boxed{
\dot{\mathbf c}_t=
\mathcal C(
\mathbf c_t,\mathbf p_t,
\mathbf k_t,\mathbf k_t^{Gc},\mathbf b_t)
}
\]

**What this means\:** The four capacities develop through practice, interaction, strategy acquisition and accumulating knowledge.

The capacity vector is\:

\[
\mathbf c_t=
\begin{bmatrix}
c_{\mathrm{Focus}}\\
c_{\mathrm{Relate}}\\
c_{\mathrm{Generate}}\\
c_{\mathrm{Learn}}
\end{bmatrix}
\]

These are the functional capacities of Trident-G\:

- Focus &amp; Control
- Relate &amp; Infer
- Generate &amp; Explore
- Learn &amp; Retain

The model allows these capacities to influence one another.

For instance, improved control may facilitate relational inference. Improved relational knowledge may facilitate subsequent learning. Better learning may support more efficient exploration.

This is the proposed mutualistic component of Trident-G.

Importantly, **the four capacities and the four entropy–mutual-information branches are not identical constructs**\. Capacities describe functional abilities, while branches describe proposed computational pathways. Their relationship must be specified and tested.

**Trident-G interpretation\:** General intelligence develops through interacting capacities whose effects can accumulate across learning episodes and environments.

This equation does not yet establish whether training increases domain-general capacity or merely improves task-specific competence. That distinction is an essential empirical question.

## 12\. Coupled niche dynamics

\[
\boxed{
\begin{aligned}
\dot{\mathbf z}_{n,t}
={}&f_n(\mathbf z_{n,t})\\
&+\sum_{m\neq n}
H_{nm}(\mathbf z_{m,t},\mathbf z_{n,t})\\
&+B_n\mathbf a_t
\end{aligned}
}
\]

**What this means\:** Environments develop through their own processes, interact with other environments and can be changed by intelligent action.

A niche might include an individual's workplace, social environment, research community or AI-supported problem-solving environment.

The function \(f_n\) represents changes arising within the niche itself.

The coupling terms \(H_{nm}\) represent interactions between niches.

The final term captures environmental modification through the agent's actions.

A person who learns to automate part of a workflow, for example, may not merely perform the existing workflow more efficiently. They may change how the workflow is organised, what information becomes available and which future actions are possible.

**Trident-G interpretation\:** Intelligent adaptation is reciprocal.

The agent learns from the environment, but also changes the environment. Those changes subsequently alter the conditions for further learning and adaptation.

This introduces niche construction into the theory and provides a mechanism by which individual intelligence could influence collective or organisational adaptation.

## 13\. Strategic action and adaptive control

\[
\boxed{
(\mathbf a_t,u_t)=
\pi(
x_t,\mathbf c_t,\mathbf k_t,
\mathbf k_t^{Gc},\mathbf r_t^\star,
\eta_t,\chi_t,\mathbf z_t)
}
\]

**What this means\:** The system selects actions and regulates its exploration–exploitation bias using its current adaptive mode, cognitive capacities, knowledge, synthesised problem representation and environmental conditions.

The policy \(\pi\) represents strategic decision-making.

It produces both externally directed actions \(\mathbf a_t\) and an internal regulatory control signal \(u_t\)\.

This closes the central cognitive–environmental feedback loop\:

**Gf synthesis and problem solving**

Near-critical generative and relational processing

**Invariant learning and Gc banking**

Validation, consolidation and efficient reuse

**Strategic action and niche transformation**

Act on the environment and modify future affordances

**Changed opportunities and adaptive demands**

New observations, uncertainty and learning conditions

Feedback into subsequent Gf synthesis

**Trident-G interpretation\:** The outcome of intelligence is not merely a correct answer. It is an adaptive action that can change both the individual and the conditions in which the individual subsequently operates.

---

# Part II. Overall interpretation

The integrated theory proposes that general intelligence emerges from the interaction of three functions.

**First, Gf provides flexible synthesis.** It coordinates the search for possibilities and the extraction of informative relationships, potentially supported by near-critical neural dynamics.

**Second, Gc provides relatively stable knowledge.** It allows successful structures to be retained, efficiently accessed and reused, potentially through more subcritical modes of processing.

**Third, homeostatic meta-control regulates their interaction.** It determines when existing knowledge is sufficient, when new exploration is warranted, when learning should occur and when environmental conditions should themselves be changed.

The outcome is a recursive process in which successful adaptation can generate knowledge and opportunities that support further adaptation.

The proposed relationship can be summarised as\:

\[
\boxed{
\begin{gathered}
\text{Regulated Gf synthesis}\\
\downarrow\\
\text{Invariant discovery and testing}\\
\downarrow\\
\text{Gc consolidation}\\
\downarrow\\
\text{Knowledge reuse and niche adaptation}\\
\downarrow\\
\text{Expanded future adaptive possibilities}
\end{gathered}
}
\]

The model therefore distinguishes *immediate adaptive performance* from *longer-term growth in adaptive capability*\.

## What would make this a scientific theory?

Four questions would be especially consequential.

| Theoretical claim | Required evidence |
|--------|--------|
| Gf uses near-critical dynamics with regulated excursions | Neural criticality measures associated with novel reasoning and switching |
| Gc preferentially supports stable, efficient processing | Evidence for differences in dynamics and task-adjusted energetic cost |
| Higher Gf improves invariant discovery | Independent Gf measures predicting relational generalisation across controlled transformations |
| Gf–Gc banking supports far transfer | Longitudinal evidence that consolidated relational structures improve later performance in different niches |

The model also needs to predict conditions under which exploration becomes maladaptive, invariants fail to transfer, or niche changes undermine rather than improve future adaptation.

These failure conditions are essential to its falsifiability.

---

# Appendix A. Trident-G coupled-dynamics model — Version 0.2

Consolidated mathematical formulation with clarified notation

The following is a compact presentation of the proposed system. The equations specify relationships between mathematical objects, but some component functions remain to be operationalised and estimated.

## Trident-G: Coupled-Dynamics Model

VERSION 0.2 · MATHEMATICAL SPECIFICATION

---

**A. Adaptive control and homeostatic regulation**

---

**B. Gf branch dynamics and criticality regulation**

Gf targets may briefly become positive under selected demands; this remains a hypothesis about neural dynamics.

---

**C. Synthesis, invariant learning and Gc banking**

\(\mathcal D_{\le t}\) denotes accumulated observations; \(\mathcal T\) denotes structure-preserving transformations used to validate candidate invariants.

---

**D. Learning, capacities and coupled niches**

---

**E. Strategic action selection**

---

Status: theoretical specification. A simulation requires explicit functional forms, compatible state representations, parameter values, initial conditions and a numerical integration method.

## Appendix B. Notation and assumptions

| Symbol | Definition |
|--------|--------|
| \(x_t\) | Adaptive mode: exploitation–exploration coordinate |
| \(\xi_t\) | Cusp stability/control parameter |
| \(\delta_t\) | Exploration–exploitation bias |
| \(\mathbf c_t\) | Four functional Trident capacities |
| \(\mathbf b_t\) | Four active Gf computational branches |
| \(\epsilon^{Gf}_{i,t}\) | Criticality-regime parameter of Gf branch \(i\) |
| \(\epsilon^{Gc}_t\) | Regime parameter associated with Gc-dominated processing |
| \(\mathbf k_t^{Gc}\) | Consolidated knowledge representation |
| \(\mathbf k_{n,t}\) | Niche-specific knowledge representation |
| \(\mathbf r_t^\star\) | Synthesised relational representation |
| \(\mathbf q_t\) | Candidate learned invariants |
| \(v_t\) | Validation strength for invariant consolidation |
| \(\eta_t\) | Meta-efficacy |
| \(\chi_t\) | Cognitive/goal coherence |
| \(\mathbf h_t\) | Internal regulatory conditions |
| \(\mathbf z_{n,t}\) | State of niche \(n\) |
| \(\mathbf a_t\) | Actions influencing niches |
| \(u_t\) | Strategic control of exploration–exploitation |
| \(F_t^\star\) | Defended regulatory reference level |

Three assumptions are particularly important.

**1\. Two different mathematical criticalities are being described.** The cusp parameter \(\xi\) controls the existence and stability of alternative adaptive states. The neural parameter \(\epsilon\) represents proximity to an activity-propagation critical boundary under a specified approximation. A mechanistic relationship between them would need to be derived, not presumed.

**2\. Stable Gc and near-critical Gf are hypotheses about processing regimes.** A knowledge store is not literally a subcritical system; the claim concerns the neural-computational dynamics predominantly recruited when knowledge is retrieved and applied. Gf and Gc processes can operate simultaneously and depend on overlapping networks.

**3\. Version 0.2 is not yet a closed dynamical system.** The quantities \(\eta_t\), \(\chi_t\), \(\mathbf h_t\) and \(F_t^\star\) currently enter as time-varying inputs rather than having their own specified evolution equations. The learning operators, transfer mappings and cost functions also require explicit forms. These are necessary additions before formal stability analysis or parameter estimation.

---

## Concluding theoretical proposition

The revised model can be expressed in a form suitable for the opening of a theoretical paper\:

> **Trident-G proposes that homeostatic general intelligence emerges from the regulated interaction of flexible, near-critical cognitive synthesis and relatively stable crystallised knowledge, operating within dynamically coupled agent–environment niches.**
>
> Fluid intelligence coordinates generative and relational computations to construct and evaluate representations of unfamiliar problems. Successful discovery of generalisable relational invariants supports their consolidation into crystallised knowledge, reducing the computational demands of subsequent problem-solving and enabling transfer across contexts.
>
> This recursive Gf–Gc–Gf cycle is regulated by homeostatic control processes that balance stability, exploration and adaptive demands. Intelligent action also modifies the niches in which cognition operates, potentially expanding the agent's future viable opportunities for learning and effective action.
>
> The theory predicts that individual differences in general intelligence will be associated not only with processing capacity, but also with the regulation of cognitive transitions, the discovery and consolidation of transferable invariants, and the ability to restructure environments in ways that support continued adaptation.

**The next mathematical priority**, in my view, is to specify the Gf synthesis operator \(\mathcal S\) and the invariant-learning mechanism \(\mathcal M\)\. Those two functions contain the strongest candidate explanation for why higher Gf might produce more generalisable knowledge, rather than merely greater speed or complexity in novel problem-solving.

---

To integrate:
**Yes. I think hierarchical modularity within a Griffiths-phase-like regime could provide a particularly useful extension of Trident-G.** It would allow us to model the simultaneous operation of automated skills, flexible problem-solving and higher-order cognitive control within a single intelligent episode.

In fact, it potentially resolves a limitation of Version 0.2: the model currently treats Gf synthesis and Gc retrieval as interacting processes, but does not adequately describe **how multiple cognitive modules can remain in different dynamical regimes while contributing to the same coordinated action**\.

My proposed development would be a **Version 0.3: Hierarchical-Modular Trident-G**, with three additional principles\:

1. **Local autonomy\:** Acquired skills and knowledge structures can operate relatively independently, without requiring continuous global cognitive control.
2. **Selective global integration\:** Gf can recruit, coordinate, interrupt or reorganise these processes when unfamiliar problems demand it.
3. **Extended criticality\:** Hierarchically organised, heterogeneous networks may sustain a mixture of localised activity, stability and long-range responsiveness over an extended range of operating conditions.

The third principle is motivated by research on Griffiths phases, especially Moretti and Muñoz (2013), who showed computationally that hierarchical modular networks can exhibit an extended critical-like region rather than requiring fine-tuning to a single critical point. [nature.com](https://www.nature.com/articles/ncomms3521)

## 1\. Why Griffiths phases are particularly relevant

In an ordinary criticality model, we might imagine an entire neural system approaching a single transition between subcritical and supercritical activity.

A Griffiths-phase account is different.

Because the network contains modules with different connectivity and local excitability, different parts can exhibit substantially different dynamical behaviour under the same global conditions.

Some regions may rapidly dampen activity; others may sustain activity for unusually long periods. These rare, locally active regions can give rise to slow relaxation and critical-like behaviour across an extended parameter range.

Relatively homogeneous network

A simplified system with similar local dynamics

Hierarchical modular network

Locally differentiated modules with selective cross-module coupling

Conceptual network illustrations. A modular architecture may support heterogeneous dynamical regimes, but modularity alone does not establish a Griffiths phase.

This is attractive for Trident-G because intelligent behaviour plainly does not require all cognitive processes to occupy the same operating mode simultaneously.

A person may perform a highly practised motor sequence automatically while using demanding relational reasoning to solve a novel problem, monitoring the consequences of their actions and maintaining a longer-term goal.

The processes are coordinated, but they do not all need the same degree of flexibility, sustained attention or conscious control.

**This suggests that criticality in Trident-G should be understood as a property of interacting multiscale systems, not simply a single global Gf state.**

## 2\. An intelligent episode can contain several processing regimes simultaneously

Consider an experienced pianist improvising during a performance.

One intelligent episode: musical improvisation

**Higher-level Gf synthesis** Flexible, novel

Develop an unexpected musical idea; anticipate how it will fit the developing piece

Selective coordination and feedback

**Relational processing**

Recognise harmony and anticipate possible transitions

**Error monitoring**

Detect unexpected outcomes and adjust timing or phrasing

Recruitment of learned skill modules

Conceptual hierarchy: multiple specialised and flexible processes contribute concurrently to one performance.

Several important things are happening\:

- Automated skills continue to function without requiring conscious specification of every action.
- Learned musical structures are retrieved and combined.
- Gf explores new possibilities and synthesises them into a coherent sequence.
- Unexpected feedback may trigger a temporary increase in cognitive control.
- Successful improvisations may become reusable musical knowledge.

This is not simply switching between Gc and Gf. **It is parallel, hierarchical coordination in which stable and flexible processes operate together.**

There is already a relevant foundation in hierarchical reinforcement learning. Botvinick and Weinstein (2014) describe how complex decision-making can incorporate temporally extended learned skills. Dezfouli and Balleine (2013) provide evidence that goal-directed processes can select learned action sequences rather than specifying every individual movement. [pubmed.ncbi.nlm.nih.gov](https://pubmed.ncbi.nlm.nih.gov/25267822/)[pubmed.ncbi.nlm.nih.gov](https://pubmed.ncbi.nlm.nih.gov/24339762/)

Trident-G could connect this established hierarchy of skilled behaviour with a theory of near-critical neural dynamics, relational synthesis and Gf–Gc knowledge banking.

## 3\. The mathematical modification: a hierarchy of interacting modules

I would introduce a collection of modules \(M_1,\ldots,M_N\), connected through a hierarchical network \(W\)\.

Each module has its own\:

- Functional state \(y_j\)\.
- Learned knowledge or skill representation \(K_j^{Gc}\)\.
- Effective criticality parameter \(\epsilon_j\)\.
- Connections with other modules \(W_{jk}\)\.
- Degree of recruitment by higher-level control \(\gamma_j\)\.

An illustrative dynamical equation would be\:

\[
\boxed{
\begin{aligned}
dy_{j,t}={}&\Big[
f_j(y_{j,t};K_j^{Gc},\epsilon_j)\\
&+\sum_kW_{jk}H_{jk}(y_{k,t},y_{j,t})\\
&+\gamma_{j,t}B_jr_t^\star
\Big]dt+\sigma_jdW_{j,t}
\end{aligned}
}
\]

This extends the earlier Gf synthesis equation.

The terms have straightforward interpretations.

**Local dynamics\:** Each module performs its specialised computations, potentially drawing on automated skills.

**Coupling\:** Modules communicate and coordinate through connections whose strengths vary across the hierarchy.

**Top-down recruitment\:** Gf synthesis selectively influences a module when its operations are needed for the current problem.

**Variability\:** Different modules can exhibit different levels of stability, responsiveness and spontaneous activity.

The important point is that modules need not operate in identical regimes.

### Griffiths-phase extension

Rather than defining a single Gf criticality parameter, we would model the distribution\:

\[
\boxed{
\boldsymbol\epsilon_t=
(\epsilon_{1,t},\epsilon_{2,t},\ldots,\epsilon_{N,t})
}
\]

The global system could exhibit a broad range of critical-like dynamics because of the interaction between heterogeneous local dynamics and hierarchical connectivity.

However, a Griffiths phase would need to *emerge from the specified network model*\. Merely assigning different criticality values to different modules would not establish one.

Research by Ódor and colleagues (2015) demonstrates that particular hierarchical network structures, with suitable connectivity conditions, can support localised activity and Griffiths phases. Other network configurations do not necessarily generate the same effects. [nature.com](https://www.nature.com/articles/srep14451)

This distinction is important for formal mathematical credibility.

## 4\. Add an explicit skill-recruitment and coordination mechanism

We now need an operation that allows Gf to recruit automated skills without necessarily taking over their detailed execution.

Let\:

\[
\boxed{
\gamma_{j,t}=
\operatorname{Gate}_j
(x_t,r_t^\star,e_{j,t},z_t)
}
\]

where \(e_{j,t}\) represents the prediction error or performance discrepancy associated with module \(j\)\.

The gate determines whether an acquired skill should be deployed, monitored more closely, modified or temporarily interrupted.

The action policy becomes\:

\[
\boxed{
a_t=
\mathcal A
\left(
a_t^{Gf},
\{\gamma_{j,t}\pi_j^{Gc}\}_{j=1}^N
\right)
}
\]

Here\:

- \(\pi_j^{Gc}\) represents a learned skill policy.
- \(a_t^{Gf}\) represents action contributions from current flexible problem-solving.
- \(\mathcal A\) coordinates these contributions into an executable action, resolving conflicts where necessary.

The formulation permits Gf and multiple Gc skill modules to contribute to the same action simultaneously.

This is preferable to a simple Gf-versus-Gc switch.

**The core adaptive capability may be knowing which operations to automate, which to monitor, and which to reconstruct through fluid reasoning.**

## 5\. Why the Griffiths-phase hypothesis adds something distinctive

Theoretically, an extended critical-like regime could provide several computational advantages.

| Dynamical property | Proposed cognitive advantage |
|--------|--------|
| Localisation of activity | Specialised skills can remain active without recruiting the entire network |
| Diverse local response times | Fast automated operations can coexist with slower integrative processes |
| Extended critical-like responsiveness | Flexible computation may remain available across changing conditions |
| Weak but consequential cross-module connections | Relevant information can sometimes influence distant processes without continuous global activation |
| Rare-region persistence | Some local activity patterns can remain influential longer than expected from simple exponential decay |

These are plausible functional interpretations, not established demonstrations that a Griffiths phase improves Gf.

The timescale aspect is particularly relevant. Evidence from cortical and limbic systems supports hierarchically organised neural timescales, with different regions integrating information over different temporal windows. [pmc.ncbi.nlm.nih.gov](https://pmc.ncbi.nlm.nih.gov/articles/PMC12060611/)[pmc.ncbi.nlm.nih.gov](https://pmc.ncbi.nlm.nih.gov/articles/PMC7755395/)

A Trident-G implementation could use these varying timescales to support rapid skilled execution, intermediate relational integration and slower monitoring of goals and niche conditions.

### A refinement of the Gc–Gf criticality hypothesis

I would now move beyond the simpler statement that Gc is subcritical and Gf supercritical.

Instead\:

**Gc-dominated skill execution** may recruit relatively stable, locally constrained dynamics, while **Gf synthesis** depends on flexible communication and integration between modules. These processes can coexist within a globally heterogeneous, near-critical network.

Some modules may exhibit local supercritical propagation without producing globally uncontrolled activation.

Importantly, stability of an automated skill does not imply that its underlying neural activity must be subcritical. Local dynamics and functional automaticity are different variables.

This is a more nuanced account that retains your original hypothesis as something testable.

## 6\. Extend Gf–Gc banking to the construction of new modules

There is one further implication that I think is especially important.

Previously, we described Gf–Gc banking mainly as the consolidation of learned knowledge and relational invariants.

But learning can also produce increasingly autonomous *computational routines*\.

The developmental sequence becomes\:

\[
\boxed{
\begin{gathered}
\text{Gf constructs a novel solution}\\
\downarrow\\
\text{Repeated successful execution}\\
\downarrow\\
\text{Consolidation into a reusable skill}\\
\downarrow\\
\text{Increasingly autonomous module}\\
\downarrow\\
\text{Selective recruitment by higher-level Gf}
\end{gathered}
}
\]

A learner initially solving a difficult problem might require sustained working memory, explicit relational reasoning and conscious monitoring.

With sufficient practice, parts of the solution may become readily retrievable or automated.

Those acquired routines can then be incorporated into more complex problem-solving episodes.

This suggests that growth of intelligence may involve not merely accumulating information but **progressively constructing a hierarchy of reusable cognitive operations**\.

It also suggests a possible explanation for cognitive efficiency: an expert can devote flexible processing resources to higher-order problems because some lower-level operations no longer require the same degree of deliberate control.

That does not necessarily mean the expert's underlying Gf capacity has increased. Greater performance could arise from more efficient skill organisation and knowledge use. The model should separate these mechanisms.

## 7\. A particularly useful Trident-G prediction

This produces a testable hypothesis that is stronger than simply predicting that higher Gf corresponds to higher neural criticality.

**People with higher Gf may be better at dynamically coordinating specialised learned modules when confronted with problems that require unfamiliar combinations of familiar skills.**

An experiment could test this using a task that first establishes several independent learned routines and then presents novel problems requiring their coordinated application.

We could compare three situations\:

1. Familiar routines executed separately.
2. Familiar routines combined in a predictable way.
3. Familiar routines combined under unexpected constraints requiring relational restructuring.

The crucial outcome would not merely be performance accuracy. It would be the ability to preserve efficient execution of familiar subroutines while flexibly reorganising their coordination.

We could measure response times, dual-task costs, switching costs, transfer and individual differences in independently assessed Gf.

An EEG extension might examine changes in network integration and localised dynamics, although scalp EEG alone would not establish the existence of a Griffiths phase.

Computationally, we could compare three models: a flat cognitive controller, a hierarchical controller without Griffiths-phase dynamics, and a hierarchical-modular controller capable of an extended critical-like regime.

The third model would need to outperform the others on preregistered predictions, rather than merely reproducing power-law-looking activity.

---

## 8\. Where this leaves the theory

I think we now have a more comprehensive architecture\:

### Trident-G Version 0.3

Hierarchical-modular, coupled-dynamical intelligence

**Meta-control and homeostatic regulation**

Maintain viability, regulate adaptive modes, allocate control resources and set goals

Control and feedback

**Gf synthesis and integrative coordination**

Explore possibilities, integrate relations, construct representations and recruit skills

Selective modular recruitment

**Hierarchically organised Gc modules**

Multiple modules can operate concurrently, with heterogeneous stability and responsiveness

Action, feedback and learning

**Coupled agent–environment niches**

Opportunities, constraints, other agents and environmental modifications

The hierarchy is functional rather than a claim that the brain contains a simple anatomical stack. In practice, there would be reciprocal and lateral connections across all levels.

### The theoretical proposition

> General intelligence emerges from homeostatically regulated coordination across hierarchically organised cognitive modules operating at different levels of stability, flexibility and temporal integration. Fluid intelligence enables novel synthesis and adaptive reconfiguration of specialised, learned processes, while crystallised intelligence provides relatively stable knowledge and reusable skills. Hierarchical network heterogeneity may facilitate this coexistence through an extended near-critical dynamical regime, allowing flexible integration without requiring global destabilisation.

**My assessment is that hierarchical modularity is not merely compatible with Trident-G; it may be an essential missing component of its mechanistic explanation.**

The important next step is to distinguish what follows from hierarchical organisation generally from what uniquely requires a Griffiths phase. Hierarchical reinforcement learning already explains much about the coordination of automatic skills and deliberate problem-solving. The distinctive additional claim would be that **extended critical-like dynamics improve the robustness and flexibility of that coordination across changing cognitive demands**\.

That gives Version 0.3 a precise theoretical contribution and, importantly, a falsifiable prediction.

--
To integrate:

**Yes. In fact, multiple interacting timescales are already central to Trident-G, and incorporating the temporal scaling properties of Griffiths phases could make Version 0.3 substantially more powerful.**

There is, however, an important distinction:

1. **Hierarchical timescales:** Different cognitive modules operate at different characteristic speeds, from rapid automated responses to slower reasoning, learning and consolidation.
2. **Critical temporal scaling:** Near criticality, the system may exhibit a broad distribution of relaxation times rather than a few fixed timescales. Some activity patterns decay rapidly, while others persist much longer.
3. **Developmental timescales:** Repeated cognitive episodes progressively alter knowledge, skills, network organisation and eventually the conditions under which future intelligence operates.

Your May 2026 Trident-G formulation already addresses all three conceptually, particularly in its sections on cross-scale successor-representation coupling and the separation of timescales. Trident_G_Theory_of_General_Ada… Trident_G_Theory_of_General_Ada…

What the proposed mathematical Version 0.3 still needs is an explicit account of **how these timescales emerge, interact and change through learning**.

That is where Griffiths-phase mathematics becomes especially interesting.

## 1. What Griffiths phases add: a continuum of timescales

In conventional models, a neural system might return to equilibrium with a characteristic relaxation time:

\[
C(t)\propto e^{-t/\tau}
\]

Here, \(\tau\) determines how quickly the system loses the influence of its previous state.

A Griffiths phase can behave differently.

Because a hierarchical network contains modules with heterogeneous connectivity, some regions can sustain activity much longer than others. The combination can produce slow, approximately power-law relaxation:

\[
\boxed{C(t)\propto t^{-\alpha}}
\]

over a finite range of timescales.

Rather than a single characteristic relaxation time, the system exhibits a broad spectrum of temporal responses. The scaling exponent can also vary within the Griffiths region.

This is central to Moretti and Muñoz's (2013) account of extended criticality in hierarchical modular brain networks. [Nature](https://www.nature.com/articles/ncomms3521?utm_source=chatgpt.com)

### Why this matters for Trident-G

Imagine an individual solving a complex problem while simultaneously:

- Executing familiar skills rapidly and automatically.
- Maintaining relevant information over several seconds.
- Integrating relational information over longer intervals.
- Monitoring a goal throughout an extended problem-solving episode.
- Updating knowledge that will influence future episodes.

These processes do not need to start and finish together.

**An extended near-critical regime could provide a dynamical substrate in which relatively independent, differently timed processes remain available for selective coordination.**

This would offer a possible physical mechanism for the hierarchical modularity we discussed.

## 2. Three nested forms of temporal organisation

For Version 0.3, I would distinguish the following:

| Scale | Illustrative duration | Trident-G function |
|---|---|---|
| Neural signalling | Milliseconds | Local excitation, inhibition and information transmission |
| Perception and control | Tens–hundreds of milliseconds | Signal selection, conflict monitoring, response preparation |
| Working-memory operations | Seconds | Maintenance, binding, updating and relational integration |
| Problem-solving episodes | Seconds–minutes | Gf synthesis, exploration, constraint and strategic switching |
| Skill acquisition | Minutes–weeks | Repeated updating and fast Gc compilation |
| Schema consolidation | Days–months | Slow Gc gist extraction and invariant integration |
| Developmental adaptation | Months–years | Changes in capacities, habitual regulation and network organisation |
| Niche evolution | Variable, potentially years | Environmental restructuring, cultural learning and collective adaptation |

These are overlapping illustrative ranges, not fixed time constants assigned to particular brain networks.

The May 2026 theory already distinguishes rapid changes in engagement and meta-control, intermediate construction of Gc schemas, and slower changes in the physiological substrate of criticality. Trident_G_Theory_of_General_Ada…

**The important new insight is that these are not simply successive stages. They are concurrently operating, reciprocally coupled processes.**

For example, a slowly changing schema can influence an immediate attentional decision. Conversely, an unexpected observation can initiate learning that eventually changes the schema.

## 3. Recent neuroscience supports the general architecture

Several studies are particularly relevant.

**Li, Li and Wang (2025)** examined cortical timescale hierarchies in marmosets. Their computational model suggested that a near-critical operating regime could support both local temporal integration and reliable information transmission between cortical regions. This is particularly relevant to coordinating modules operating at different speeds. [Nature](https://www.nature.com/articles/s41467-025-66699-4?utm_source=chatgpt.com)

**A 2025 human intracranial EEG study** found that cortical timescales change between wakefulness and sleep, with different patterns for broadband and gamma activity. This supports treating timescales as dynamic properties rather than fixed characteristics of anatomical regions. [PubMed Central (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC11984084/?utm_source=chatgpt.com)

**Zeraati and colleagues (2026)** provide an especially relevant computational review. They emphasise that neural timescales vary within and between brain regions, while distinguishing observed temporal hierarchies from the mechanisms proposed to generate them. [Nature](https://www.nature.com/articles/s41593-026-02343-8?utm_source=chatgpt.com)

Together, these results make a multiscale Trident-G architecture plausible. They do not establish that the brain operates in a Griffiths phase during fluid reasoning or that its timescale distribution determines Gf.

---

# 4. The mathematical addition to Version 0.3

I would introduce an explicit timescale parameter for each cognitive module.

Let module \(j\) have state \(y_j\), characteristic response time \(\tau_j\), and a local cusp-like potential \(V_j\).

We can write:

\[
\boxed{
\tau_j\frac{dy_j}{dt}
=
-\frac{\partial V_j}{\partial y_j}
+
\sum_k W_{jk}H_{jk}(y_k,y_j)
+
\gamma_j r_t^\star
+
I_j(t)
}
\]

This is the deterministic component; stochastic fluctuations can be added as in Version 0.2.

The terms represent:

- \(\tau_j\): characteristic response time of module \(j\).
- \(V_j\): its local dynamical landscape.
- \(W_{jk}\): hierarchical coupling with other modules.
- \(\gamma_j\): recruitment by current Gf synthesis.
- \(r_t^\star\): the synthesised relational representation.
- \(I_j(t)\): local task or environmental input.

A rapid automated module might have a short response time.

A module integrating information over a longer horizon might have a larger effective response time.

The modules can operate simultaneously, with their coupling determining which information propagates through the hierarchy.

### From multiple timescales to Griffiths-phase dynamics

Merely assigning different \(\tau_j\) values would generate a multiscale system, but not necessarily a Griffiths phase.

For the stronger Griffiths-phase hypothesis, the network needs an appropriate combination of hierarchical connectivity, heterogeneity and locally persistent activity.

One way to characterise the resulting dynamics is through a distribution of effective relaxation times:

\[
\boxed{
P(\tau)\propto\tau^{-(1+\alpha)}
}
\]

over some interval \([\tau_{\min},\tau_{\max}]\).

A weighted mixture of exponential relaxation processes with this distribution can produce:

\[
C(t)\propto t^{-\alpha}
\]

over an intermediate scaling range.

This is an illustrative representation of broad temporal scaling, not a sufficient condition for a Griffiths phase.

The mathematical task would be to determine whether the observed distribution emerges from the hierarchical modular network itself.

---

## 5. Add learning-dependent changes in timescales

This is potentially the most important extension for Trident-G.

As people learn, the organisation of cognitive processing changes.

Operations that initially require slow, deliberative processing can become faster, more autonomous and easier to coordinate.

But learning can also create longer-horizon representations that integrate information across increasingly extended periods.

Thus, learning need not simply make all processing faster.

**It may simultaneously produce faster lower-level operations and deeper, longer-timescale integration at higher levels.**

We can model experience-dependent changes in a module's characteristic timescale:

\[
\boxed{
\frac{d\tau_j}{dt}
=
\mathcal T_j
\left(
\tau_j,
K_j^{Gc},
P_j,
W,
\mathbf z
\right)
}
\]

Here, the evolution of \(\tau_j\) depends on consolidated skill, practice, network organisation and niche conditions.

Importantly, this equation is a proposed developmental mechanism, not an established law of learning.

It permits two complementary changes:

**Compilation:** A repeated operation becomes faster and more autonomous, reducing the time and control required for its execution.

**Temporal integration:** Higher-level representations develop the ability to incorporate more distant information and longer chains of consequences.

The result could be a progressively differentiated hierarchy of cognitive timescales.

### Connection with successor representations

This connects directly with the three levels of SR processing in the May 2026 Trident-G theory:

- Fast subcortical SR automations.
- Intermediate hippocampal predictive maps.
- Slower prefrontal schemas.

The theory already proposes bidirectional interactions between these levels. Trident_G_Theory_of_General_Ada…

There is also a useful mathematical distinction here.

An SR's **predictive horizon** is not identical to the **neural relaxation time** of the system representing it.

For instance, a neural computation lasting a fraction of a second could retrieve a model predicting consequences several years ahead.

The more general formulation should therefore include both:

\[
\boxed{
\begin{aligned}
\tau_j &= \text{processing timescale}\\
h_j &= \text{predictive horizon}
\end{aligned}
}
\]

Their coupling could become an important Trident-G research question.

---

# 6. A deeper implication: Gf might coordinate temporal horizons

This suggests a potentially distinctive interpretation of fluid intelligence.

Previously, we described Gf as coordinating entropy-generating and mutual-information-extracting processes.

Now we can add that it must coordinate **different temporal horizons**.

Consider a chess player.

A familiar board configuration can rapidly activate learned patterns and procedures.

An unfamiliar position requires active exploration and relational reasoning.

At the same time, the player must integrate immediate tactical consequences with longer-term positional considerations.

Higher Gf might therefore support the ability to construct and coordinate models extending across several temporal horizons.

For example:

\[
\boxed{
r_t^\star=
\mathcal S
\left(
\mathbf b_t,
K_t^{Gc},
\{SR_{h_1},SR_{h_2},\ldots,SR_{h_n}\}
\right)
}
\]

Here, \(SR_{h_i}\) represents predictive structure at horizon \(h_i\).

The synthesis operator coordinates these representations into a usable problem model.

A person with higher Gf might be better able to identify a relational invariant that connects a short-term event to a much longer sequence of consequences.

This would extend your invariant-learning hypothesis:

**Higher Gf may support not only invariant discovery across different contexts, but also invariant discovery across different temporal scales.**

That is an interesting and testable proposition.

---

## 7. The relationship with Gc banking

The timescale formulation also improves the Gf → Gc → Gf model.

Previously, we described Gc banking mainly as the consolidation of knowledge.

But consolidation can also change the temporal organisation of future computation.

A newly learned operation may initially require multiple slow, attention-demanding steps.

After compilation, those steps can be executed as a faster, more integrated routine.

This releases resources for higher-order Gf synthesis.

Meanwhile, slower gist extraction may integrate patterns across multiple learning episodes, producing representations that support longer-horizon reasoning.

The cycle becomes:

\[
\boxed{
\begin{gathered}
\text{Gf synthesis across timescales}\\
\downarrow\\
\text{Invariant discovery}\\
\downarrow\\
\text{Fast Gc skill compilation}\\
+\quad
\text{Slow Gc schema integration}\\
\downarrow\\
\text{Changed temporal organisation}\\
\downarrow\\
\text{Richer subsequent Gf synthesis}
\end{gathered}
}
\]

This provides a possible mechanism for the developmental spiral already proposed in Trident-G.

It also suggests that growing intelligence may involve changes in **the distribution and coordination of computational timescales**, not merely increases in processing capacity.

---

# 8. An important prediction for Version 0.3

We can now distinguish three competing models.

| Model | Main assumption | Predicted temporal dynamics |
|---|---|---|
| Single-scale model | Cognition is governed by a dominant response time | Relatively simple exponential relaxation |
| Hierarchical multiscale model | Different modules operate at different characteristic speeds | Multiple distinguishable response times |
| Griffiths-phase hierarchical model | Heterogeneous modular interactions generate extended critical-like dynamics | Broad relaxation-time distributions and extended scaling behaviour |

The third model makes an additional prediction.

When the system encounters novel problems requiring combinations of automated skills and flexible reasoning, **the heterogeneous near-critical model should maintain effective coordination across a wider range of demands** than otherwise comparable models without the Griffiths-phase regime.

We could examine this through computational simulations and, eventually, combined EEG and behavioural experiments.

Relevant outcomes would include temporal autocorrelations, relaxation times following perturbations, persistence of task representations, efficiency of modular recruitment, switching costs and delayed transfer.

Crucially, observing approximately \(1/f\) spectra or power-law correlations would not by itself establish a Griffiths phase. Other multiscale processes can generate similar statistics. The model would need comparisons against noncritical alternatives and evidence of an extended critical-like operating region.

---

# 9. A final refinement to the mathematical architecture

I would now distinguish **three levels of mathematical description**:

| Mathematical component | Function |
|---|---|
| **Cusp dynamics** | Models local attractor structure, commitment and bifurcations |
| **Griffiths-phase hierarchical dynamics** | Models heterogeneous modular activity and extended temporal scaling |
| **Slow learning and structural dynamics** | Models how skills, representations, regulatory parameters and networks change over time |

These components are complementary rather than interchangeable.

One notation correction is important for consistency with the original Trident-G theory: the cusp state remains \(x=F-F^\star\), the deviation from the defended set-point, while \(\delta\) controls the explore–exploit tilt. The earlier suggestion that \(x\) itself simply runs from exploitation to exploration should not replace those established meanings. LifeontheCusp_TheTridentGTheory…

## The emerging theoretical principle

The strongest formulation may be:

> **General intelligence depends on the capacity to coordinate and progressively reorganise cognitive processes across multiple spatial and temporal scales, maintaining the stability of specialised learned operations while enabling flexible near-critical synthesis when novel problems demand it.**
>
> Hierarchical modularity permits relatively autonomous processes to coexist. Griffiths-phase-like dynamics may provide an extended regime in which these processes can communicate and reorganise without global destabilisation. Learning changes the temporal and relational organisation of the hierarchy, allowing previously demanding operations to become efficient computational building blocks while higher-order cognition integrates information across increasingly complex contexts and predictive horizons.

**I think this is a significant refinement of Trident-G.** It suggests that *g* might be related not simply to near-criticality or the capacity for relational inference, but to the **breadth, coordination and developmental reorganisation of the cognitive system's effective timescales**.

That leads to a particularly interesting research question:

**Does higher Gf predict a greater capacity to coordinate information across multiple temporal horizons, independently of processing speed, working-memory capacity and existing Gc?**

This would be a strong candidate for one of Version 0.3's central falsifiable predictions.
