# Trident-G: A Hierarchical, Multiscale Theory of Homeostatic General Adaptive Intelligence

**Unified working theory — Version 0.3 (13 November 2026)**  
**Author:** Mark Ashton Smith  
**Status:** Conceptual and mathematical research programme; not an empirically validated account of general intelligence.

> **Core proposition.** General adaptive intelligence arises from the regulation of a heterogeneous, hierarchically organised agent–environment system. Relatively stable, reusable Gc representations and skills operate concurrently with flexible Gf synthesis. Homeostatic control regulates which processes remain autonomous, which are recruited, and when established structures must be reconsidered. Learning changes the knowledge, modular organisation and temporal horizons available for future cognition; action also changes the niches in which the system learns.

This document consolidates the three earlier sections of this file—coupled-dynamical Trident-G v0.2, hierarchical modularity/Griffiths phases, and multiscale temporal dynamics—into **one account**, rather than three consecutive extensions. Its equations are an explicit modelling scaffold, not a claim that the underlying neural mechanisms have been demonstrated.

---

## Abstract

Trident-G proposes that general intelligence is best understood as **viable, self-modifying adaptive control** across cognitive and environmental scales. A defended homeostatic corridor, $F^\star$, constrains effective engagement, while a cusp-like control landscape permits persistence, strategic switching, hysteresis and recovery. Within that landscape, Gf is conceived as flexible synthesis across entropy-oriented search and mutual-information-oriented constraint, operating over internal and externally anchored representations. Gc supplies consolidated relational knowledge, schemas, strategies and increasingly autonomous skills. These processes occur **simultaneously** within intelligent episodes: Gf can recruit several Gc modules, coordinate them at unfamiliar interfaces, and reopen their assumptions when prediction errors warrant it.

The neural implementation is hypothesised to be hierarchically modular and dynamically heterogeneous. Under particular connectivity and activation conditions, such networks may exhibit **Griffiths-phase-like extended criticality**: localised persistence and a broad range of relaxation times across an extended parameter interval. This hypothesis is distinct from both the cusp bifurcation and the more general claim that cognitive processes operate at different speeds. Learning generates candidate relational invariants, tests their portability and selectively banks them through fast skill/policy compilation and slower schema or gist integration. Accumulated changes reshape later problem-solving, module recruitment, predictive horizons and interaction with coupled niches.

The model predicts individual differences in regulated state transitions, novel composition of familiar skills, invariant learning, cross-timescale coordination, delayed transfer and recovery from perturbation. Its distinctive claims require comparison against noncritical hierarchical and conventional reinforcement-learning models, as well as independent psychometric and neural measurements.

---

> **Neuroscientific substrate hypothesis.** A replicated frontoparietal distinction provides a candidate route for the internal/external axis: **FPCN-A preferentially couples with the default network (internally directed and future-oriented processing), while FPCN-B preferentially couples with the dorsal attention network (externally directed and perceptual-task processing)**. The four entropy/MI computational branches, their Gf synthesis and the full homeostatic cusp remain Trident-G hypotheses rather than experimentally established equivalents of these networks (Dixon et al., 2018; Murphy et al., 2020; Nee, 2021; Yin et al., 2022).

# 1. The explanatory problem and the proposed solution

Traditional psychometric descriptions of fluid intelligence (Gf) and crystallised intelligence (Gc) identify important dimensions of performance, but do not by themselves specify how an intelligent *episode* is organised or how repeated episodes change future competence. A person can type, read, recall known procedures and recognise familiar patterns while simultaneously reasoning about a novel problem. Some components are fast and well learned; others demand active restructuring. The same episode may span milliseconds of sensory processing, seconds of working-memory coordination, minutes of problem solving, and the much longer interval over which the resulting lesson is consolidated.

Trident-G treats these facts as different aspects of a **single coupled dynamical process**. The proposed explanatory task is to show how an agent:

1. maintains a viable operating state under changing demands;
2. combines autonomous learned operations with flexible novel reasoning;
3. explores possibilities while selectively constraining them with informative evidence;
4. coordinates representations and actions across several processing and predictive timescales;
5. discovers useful invariants rather than retaining only task-specific answers;
6. converts validated structures into reusable skills, schemas and strategies;
7. transfers these structures across altered contexts and niches; and
8. changes its own developmental conditions by acting on its environments.

The theory is not that more activation, greater uncertainty, longer memory or stronger criticality is *always* better. Its claim is that **adaptive regulation of heterogeneous resources** matters: exploit established structures when appropriate; reopen them when changed evidence matters; preserve viable action and future learning opportunities while doing so.

## 1.1 Levels of explanation

Three mathematical descriptions are complementary, not interchangeable.

| Description | Principal object | Proposed explanatory role |
|---|---|---|
| **Cusp / homeostatic control** | Mesoscopic state and control variables $x,\xi,\delta$ | Persistence, commitment, switching, hysteresis and access to a viable Ψ-band |
| **Hierarchical modular network dynamics** | Interacting modules $y_j$, topology $W$, local propagation regimes $\zeta_j$ | Concurrent skilled and flexible processing; selective recruitment; potential extended critical-like dynamics |
| **Learning, consolidation and niche dynamics** | Knowledge $K$, capacities $\mathbf c$, timescales $\tau$, predictive horizons $h$, environments $\mathbf z$ | Transfer, development, structural reorganisation and recursive Gf→Gc→Gf growth |

The cusp does **not** mathematically prove neural criticality. Hierarchical modularity does **not** by itself imply a Griffiths phase. A power law in behavioural or neural data does **not** by itself demonstrate a Griffiths phase or intelligence-related benefit.

## 1.2 Functional capacities versus computational branches

The four **Trident capacities** are Focus & Control, Relate & Infer, Generate & Explore, and Learn & Retain. They are hypothesised functional abilities and can participate in many tasks.

The four **Gf computational branches**, defined below, describe a *different* cross-classification: internal versus external processing crossed with entropy-oriented search versus mutual-information-oriented constraint. A capacity may recruit more than one branch; a branch may contribute to more than one capacity. Neither taxonomy should be treated as four established, non-overlapping anatomical modules.

---

# 2. Homeostatic regulation and cusp geometry

The original Trident-G control variables are retained:

$$
x_t=F_t-F_t^\star,\qquad
\xi_t=G_t-F_t^\star,\qquad
\varepsilon_t=F_t-G_t=x_t-\xi_t.
$$

Here $F_t$ is a coarse-grained **realised regulatory burden**, $G_t$ its **anticipated counterpart**, and $F_t^\star$ the defended reference level. The signed mismatch $\varepsilon_t$ indicates whether realised conditions are more or less demanding than anticipated. These quantities must be placed on a common operational scale; their identification with variational free energy and expected free energy in standard active inference is **not automatic**. The letter $G$ here is anticipated load and should not be confused with psychometric general intelligence $g$.

The canonical cusp potential is:

$$
\boxed{V(x;\xi,\delta)=x^4-\xi x^2-\delta x.}
$$

Its simplest stochastic gradient dynamics are:

$$
\boxed{
dx_t=\left(-4x_t^3+2\xi_t x_t+\delta_t\right)dt+\sigma_x\,dW_t^{(x)}.
}
$$

The state $x$ remains the deviation from $F^\star$; **it is not a direct exploration–exploitation axis**. The control parameter $\xi$ governs the shape of the potential and the availability of alternative stable equilibria. The tilt $\delta$ biases the dynamics towards one attractor relative to another. In the intended psychological reading, the sign of $\delta$ denotes a conventionally specified exploration/convergence preference; no fixed mapping from the sign of $x$ to a cognitive process is assumed.

For the normalised potential, equilibria satisfy $4x^3-2\xi x-\delta=0$. Two stable minima separated by one unstable equilibrium are possible when $\xi>0$ and $27\delta^2<8\xi^3$; the folds lie on $27\delta^2=8\xi^3$. These are **cusp conditions**, not neuronal branching thresholds.

### Interpretation

A practised approach may persist despite small changes in demand. Under gradually increasing evidence for a different approach, the agent can eventually switch modes, sometimes abruptly. The return threshold need not equal the departure threshold (hysteresis). Noise can also trigger transitions before a deterministic fold.

A favourable cognitive episode is not defined by occupying a particular well indefinitely. It is defined by **appropriate deployment and recovery**: maintaining viable engagement, preserving useful automations, accessing flexible reconfiguration where warranted, and returning to efficient execution or consolidation afterwards.

The proposed **Ψ-band** is the operational region in which such transitions are sufficiently accessible and sustainable. It remains a theoretical corridor to be operationalised in behavioural and physiological data, not a directly observed location in state space.

### Regulation by capacities and niches

The expected-demand state $G_t$ may depend on capacities, meta-efficacy, coherence, knowledge and context:

$$
G_t=\mathscr G(\mathbf c_t,\eta_t,\chi_t,\mathbf h_t,
K_t^{Gc},\mathbf b_t,\mathbf z_t,\text{goal}_t).
$$

Accordingly, $\xi_t=G_t-F_t^\star$. This is a hypothesis about how anticipated demand is formed; $\mathscr G$ is not psychometric $g$.

### Candidate neural substrate for homeostatic/allostatic regulation

**Evidence.** Human neuroimaging and nonhuman anatomical tract-tracing support a distributed allostatic–interoceptive system incorporating anterior/midcingulate and insular cortices, default-mode and salience-associated regions, with connections to autonomic and brainstem regulatory circuitry. Kleckner et al. (2017) combined anatomical priors with replicated human functional-connectivity analyses; Zhang et al. (2025) extended the anatomy with 7-Tesla fMRI (n = 90) and greater subcortical resolution. Sridharan, Levitin and Menon (2008) found evidence implicating right fronto-insular cortex in switching between executive and default-mode networks.

**Trident-G hypothesis.** Salience, interoceptive and visceromotor circuitry contributes estimates of bodily/regulatory condition and the salience of mismatches, while control systems adjust engagement and policy selection. This offers a plausible *candidate substrate* for the \(F,F^\star,G,\eta,\chi\) control variables, but none of those scalar quantities is directly decoded or uniquely identified by the cited connectivity experiments. Anterior insula, ACC, LC–noradrenaline and striatum should not be assigned one-to-one to \(\xi\), \(\delta\) or \(F^\star\) without an explicit measurement model.

**Possible measurements.** Simultaneously sample task performance, pupil/arousal measures, autonomic indices and source-resolved neural network dynamics where feasible. Model whether interoceptive/autonomic signals prospectively predict successful re-entry after perturbation; do not treat HRV, pupil diameter or a particular oscillatory exponent as a unique biomarker of \(F^\star\).

### A prediction-error-modulated tilt: connecting dopamine to cognitive control

The original Trident-G account proposes that better-than-expected outcomes tend to reinforce effective policies, while worse-than-expected outcomes can suppress unsuccessful policies and prompt re-evaluation. That proposal has a substantial foundation in dopamine reward-prediction-error (RPE) research, but its extension to the mutual-information/entropy arms must remain a **separately testable hypothesis**.

Many dopamine neurons increase phasic firing when reward exceeds expectation and decrease firing when expected reward fails to occur (Schultz, Dayan, & Montague, 1997). In influential basal-ganglia models, dopamine increases preferentially support D1-associated direct/Go-pathway plasticity, while dopamine decreases reduce D2 receptor stimulation and can **disinhibit** indirect/NoGo-pathway neurons. This predicts different contributions to positive- and negative-outcome learning; human Parkinson's, PET and mouse causal studies provide important converging evidence (Frank, Seeberger, & O'Reilly, 2004; Kravitz, Tye, & Kreitzer, 2012; Cox et al., 2015; Lee et al., 2021).

Two restrictions are essential. First, a **dopamine dip is not increased D2 receptor activation**. Second, D1-expressing cells are not universally positive-value encoders and D2-expressing cells are not universally negative-value encoders: for example, nucleus-accumbens studies have found valence-independent and cooperative signals (Zachry et al., 2024). Recent distributional reinforcement-learning work suggests D1 and D2 populations can preferentially represent different *tails of reward distributions*, not simply two discrete outcome labels (Lowet et al., 2025). Reward-based learning, motivational vigour, directed information-seeking and novelty-related learning also recruit partly different mechanisms.

To keep these distinctions explicit, use a *reward* prediction error separate from the existing allostatic mismatch:

$$
\Delta_t^{R}=r_t-\widehat r_t,\qquad
\ell_t^{+}=\alpha_{+}[\Delta_t^{R}]_{+},\qquad
\ell_t^{-}=\alpha_{-}[-\Delta_t^{R}]_{+},
$$

where $[v]_{+}=\max(v,0)$. The terms $\ell^{+}$ and $\ell^{-}$ are **effective learning signals**, not measured D1 or D2 receptor activation. Their relative gains may depend on tonic dopamine, striatal region, receptor properties and previous learning. In particular, $\Delta_t^{R}$ is a reward/outcome-value error and must **not** be identified with Trident-G's $\varepsilon_t=F_t-G_t$, which is a regulatory burden mismatch.

Define the contextual baseline tilt:

$$
\delta_t^{\mathrm{base}}
=u_t+\sum_n\lambda_{n,t}\psi_n(\mathbf z_{n,t},K_{n,t})
+\boldsymbol\omega^\top\mathbf b_t.
$$

An **illustrative** trial-wise control update is:

$$
\boxed{
\begin{aligned}
\delta_{t+1}=\mathrm{clip}\Big[
&\rho_\delta\,\delta_t+(1-\rho_\delta)\,\delta_t^{\mathrm{base}}\\
&+\beta_{+}g_t^{+}\ell_t^{+}
-\beta_{-}g_t^{-}\ell_t^{-}\\
&+\beta_{C}S_t-\beta_{E}\mathrm{EIG}_t
\Big],
\end{aligned}
}
$$

where positive $\delta$ is **conventionally defined** as a bias towards continued/convergent policy use, and negative $\delta$ as a bias towards reopening/divergent search (the sign convention adopted in the 2025 Trident-G account). This is a **phenomenological assignment of control bias**, not an identity between the sign of $x=F-F^\star$ and exploration/exploitation. In the stated cusp potential, a positive $\delta$ mechanically favours higher $x$ (greater positive deviation from the defended reference), not exploitation *as such*. A validated mapping from policy bias to allostatic displacement is still required; if it proves inconsistent across tasks, the model should introduce a separate policy-mode coordinate rather than redefining $x$. In this proposal:

- $\rho_\delta$ represents persistence of the previous control bias.
- $g_t^+$ and $g_t^-$ are context-sensitive gates evaluating whether the outcome is genuinely diagnostic for retaining or revising the **current model or policy**.
- $\beta_+g_t^+\ell_t^+$ represents a *candidate* D1/Go-sensitive contribution to reinforcing an adequately supported current policy.
- $-\beta_-g_t^-\ell_t^-$ represents a *candidate* dopamine-dip/indirect-pathway-sensitive contribution to suppressing or reconsidering an unsuccessful policy; **it does not automatically cause exploration**.
- $S_t$ denotes independent evidence supporting the current model (a candidate mutual-information-related constraint signal, not mutual information itself).
- $\mathrm{EIG}_t$ is the expected information gain from testing alternatives; when high it can favour *directed* exploration, even without negative reward feedback.
- The $\beta$ coefficients are unknown, non-negative, task-dependent gains to be estimated, and clip imposes a specified safe or numerically bounded range.

This formulation distinguishes **learning from an outcome**, **whether a policy should be retained**, and **whether wider search is worth undertaking**. A disappointing outcome may justify switching to another well-learned response without generating new hypotheses. Conversely, a surprising success may reveal a new affordance that makes additional exploration desirable. Therefore, prediction-error valence should *modulate* $\delta$ rather than mechanically determine its sign.

**What is empirically supported?** Dopamine RPEs and outcome-sensitive direct/indirect pathway plasticity are well studied. **What remains a Trident-G claim?** That these signals, combined with uncertainty, expected information gain, coherence and current goals, tune the cusp's explore–exploit tilt and control entropy-oriented versus mutual-information-oriented cognitive operations. Frank et al. (2009) provide a particularly important caution: striatal dopaminergic genes were associated with outcome-based exploitative updating, while a prefrontal dopamine-related gene was associated with uncertainty-sensitive *directed exploration*. This is a reason to keep the epistemic term separate from the striatal RPE terms.

More coupling is not always better: inaccurate, captured or hostile niche coupling may also distort the tilt.

**Boundary of the claim.** A cusp is a candidate low-dimensional *control approximation*. Its parameters must be fitted and compared with smooth state-space, reinforcement-learning and switching alternatives before interpreting observed behavioural shifts as cusp bifurcations.

---

# 3. Hierarchical modularity: skilled and fluid processing in one episode

An intelligent episode contains a **population of partially autonomous computational modules**, not a homogeneous global cognitive state. Some modules implement readily available Gc skills, policies and schemas. Others participate in novel inference, evaluation or control. They interact laterally and hierarchically, with top-down recruitment and upward prediction-error signals.

Let $M_j$ denote module $j$, with state $y_j(t)$, locally available knowledge $K_j^{Gc}$, network couplings $W_{jk}$, recruitment gate $\gamma_{j,t}\in[0,1]$ and characteristic processing timescale $\tau_j>0$. An illustrative local dynamics is:

$$
\boxed{
\begin{aligned}
\tau_j\,dy_{j,t}={}&\Big[
f_j(y_{j,t};K_j^{Gc},\zeta_{j,t})
+\sum_kW_{jk}H_{jk}(y_{k,t},y_{j,t})\\
&+\gamma_{j,t}B_j\mathbf r^\star_{t^-}
+I_j(t)
\Big]dt+\sigma_j\,dW^{(j)}_t .
\end{aligned}
}
$$

The term $f_j$ represents local computation; $H_{jk}$ represents interactions; $I_j$ represents inputs; $\gamma_j B_j\mathbf r^\star$ permits higher-level Gf synthesis to recruit or reconfigure module $j$. The notation $t^-$ indicates the previous available synthesis estimate, avoiding a circular instantaneous definition of recruitment and synthesis.

Different modules can remain active at once, with different levels of autonomy and responsiveness. **An automated skill is not equivalent to a globally subcritical brain state**; automaticity is a functional property, while criticality is a dynamical property to be measured.

## Neural evidence for modular autonomy and integration

A network account is supported more directly than a strict cognitive-module-to-region correspondence. **Bertolero, Yeo and D'Esposito (2015)** examined 9,208 experiments spanning 77 cognitive tasks and found that activity in between-module connector regions increased with the number of recruited functions, whereas more local network nodes showed comparatively independent engagement. **Cole et al. (2013)** demonstrated that the frontoparietal network changes its brain-wide functional-connectivity configuration across tasks, consistent with flexible hubs that support adaptive control. These are observational and meta-analytic findings, not proof that a particular region is the unique Gf supervisor.

A particularly close mechanistic precedent is **Murphy et al. (2020)**: using 2-back fMRI and diffusion data from 644 Human Connectome Project participants, they identified frontoparietal subdivisions preferentially aligned with DMN or DAN, related functional/structural coupling to working-memory performance, and explored the resulting dynamics with coupled oscillators. **Nee (2021)** further showed an external/present-to-internal/future control gradient in frontoparietal cortex, with an intermediate integrative zone associated with individual cognitive differences. These findings motivate a flexible, distributed recruitment architecture rather than a single central executive that simply turns whole networks on or off.

**Learning modifies modular organisation:** Bassett et al. (2011) measured changing fMRI network communities across training of a motor sequence and found that flexibility of module allegiance in one session predicted learning in a subsequent session. This supports experience-dependent network reconfiguration, but does not establish that motor-skill learning improves general intelligence or that increased modular flexibility always helps.

**Trident-G implication:** the module coupling matrix \(W\) and recruitment gates \(\gamma_j\) should be constrained using task-dependent network data. Local autonomy and connector-mediated integration are empirically supported *organisational features*; the proposed causal Gf control law remains to be estimated.

## 3.1 Selective recruitment and joint action

A module's recruitment depends on task cues, the current plan, context and evidence of mismatch:

$$
\gamma_{j,t}=\mathrm{Gate}_j
(\mathbf o_{t^-},\mathbf r^\star_{t^-},e_{j,t^-},\mathbf z_t,\eta_t).
$$

The action assembled from concurrent processes is:

$$
\boxed{
\mathbf a_t=\mathcal A\Big(
\mathbf a^{Gf}_t,\{
\gamma_{j,t}\pi_j^{Gc}(\mathbf o_t)
\}_{j=1}^{N}
\Big).
}
$$

Thus Gf can **select, combine, monitor, interrupt or revise** Gc policies without performing every low-level operation itself. The assembly operator $\mathcal A$ must resolve incompatible actions and allocate available resources; it is not assumed to be effortless or unlimited.

A module can be highly active while receiving little global attention. Conversely, an error in a normally automatic module may cause targeted recruitment of Gf. Local failure need not force a global restart: the spread of corrective processing should depend on whether the mismatch threatens the current goal, policy or higher-level model.

## 3.2 Example: scientific problem-solving

A scientist developing an unfamiliar experiment can simultaneously use learned statistical procedures, familiar reading and writing operations, domain schemas, explicit relational reasoning and generative hypothesis testing. Rapid routine operations and slower inference contribute to the *same* episode. An anomalous result may reopen one assumption, which can in turn alter the experiment, the interpretation of evidence and eventually the research niche.

The meaningful hierarchy is not “first Gc, then Gf”. It is **parallel skilled operation with conditional higher-level integration**, followed by selective consolidation of whatever survives testing.

---

# 4. Neural criticality and the Griffiths-phase hypothesis

The model distinguishes *cusp bifurcation* from a separate proposed measure of **local activity-propagation criticality**. For an idealised branching approximation, define:

$$
\boxed{\zeta_{j,t}=m_{j,t}-1,}
$$

where $m_j$ estimates effective activity propagation in module $j$. Then $\zeta_j<0$, $=0$, and $>0$ correspond to subcritical, critical and supercritical propagation **within that particular approximation**. Neither $\zeta$ nor $m$ is directly inferred from an intelligence score, and $\zeta$ should not be confused with the allostatic mismatch $\varepsilon=F-G$.

### The Gf/Gc regime hypothesis

The proposed distinction is **relative and task-conditional**. Retrieval or performance of well-learned Gc skills may often rely on locally constrained, more stable processing; novel Gf synthesis may recruit modules operating near criticality, sometimes with transient more strongly propagating activity. But Gf and Gc are not separate anatomical systems, and neither is assigned a compulsory criticality sign.

The proposed claim that efficient Gc execution has a lower *incremental task cost* than constructing a novel solution is also conditional on comparable task outcomes and expertise. It does not follow merely from a negative $\zeta_j$, nor does it assert that Gc entails lower total brain energy consumption.

## Empirical evidence linking critical-like dynamics to cognitive performance

**Human correlational evidence.** Ezaki et al. (2020) fitted a statistical-physics-inspired model to resting-state fMRI and reported that participants with higher performance/fluid-type IQ measures tended to lie nearer a modelled critical boundary, with only a **moderate** association. Xu, Feng and Yu (2022) reported associations between individualised avalanche/synchronisation statistics and *fluid intelligence and working memory*, but not their crystallised-intelligence measure; they also found longer average occupancy of slightly subcritical states. These are encouraging tests of a proposed Gf/Gc *difference*, not direct demonstrations that a Gf process is supercritical and a Gc module is subcritical.

**Task specificity.** Liu, Fei and Liu (2025; online December 2024) reported that perceptual tasks selectively shifted criticality estimates of relevant cortical subsystems; their findings favour task- and region-dependent regulation over global, uniform criticality. Müller et al. (2025) used multiday intracranial EEG in people with epilepsy and associated departures from critical dynamics with cognitive impairment, while observing perturbations linked to medication, interictal events and sleep-like episodes. The clinical sample and inference method limit generalisation to healthy fluid intelligence.

**Important counterevidence and alternatives.** Priesemann et al. (2014) reported in-vivo spike-avalanche evidence consistent with a driven, **slightly subcritical** state. Criticality proxies depend on model class, recordings, preprocessing, finite sampling and observation timescale; apparent power laws can have noncritical explanations. None of these human studies demonstrates that a *Griffiths phase*, rather than another near-critical mechanism, uniquely supports Gf or Gc. Moretti and Muñoz (2013) offer a relevant **computational network model**, not empirical identification of a Griffiths phase in human reasoning.

The proposed four-way separation remains: **(i)** stable or automated task behaviour, **(ii)** a cusp-like control transition, **(iii)** a local branching/propagation regime, and **(iv)** an extended Griffiths-phase region. No one observation licenses equating them.

## 4.1 Why Griffiths phases matter

In sufficiently heterogeneous and hierarchically modular networks, rare locally active regions can sustain activity for unusually long periods while other regions relax rapidly. Some dynamical models of such networks exhibit **extended Griffiths phases**, in which critical-like behaviour occurs over an interval of control parameters rather than only at a finely tuned point (Moretti & Muñoz, 2013; Ódor and colleagues, 2015).

A network-level hypothesis is therefore:

> Hierarchical heterogeneity may widen the operating conditions under which specialised modules can remain functionally differentiated yet selectively communicate during unfamiliar, integrated problems.

This would be useful for Trident-G because it offers a *possible implementation* of concurrent skilled autonomy and flexible synthesis. But an extended critical-like regime cannot be declared from heterogeneous $\zeta_j$ values alone. It must **emerge from explicit local dynamics and network topology**.

## 4.2 From response times to broad temporal scaling

A single relaxation process can decay approximately exponentially:

$$
C(t)\propto e^{-t/\tau}.
$$

In a system with a sufficiently broad distribution of effective relaxation times, a mixture of such responses can exhibit an intermediate power-law-like regime:

$$
P(\tau)\propto\tau^{-(1+\alpha)}
\quad\Longrightarrow\quad
C(t)\propto t^{-\alpha}
$$

over a bounded range under suitable weighting and scale separation. This illustrates the difference between **multiple fixed timescales** and **scale-rich temporal organisation**.

Such a pattern is *compatible* with Griffiths-like dynamics, but not diagnostic of them. Long-memory stochastic processes, mixtures of ordinary exponentials, filtering and nonstationarity can produce similar signatures. A credible test requires model comparison, finite-size analysis and evidence for an extended parameter region with suitably localised slow activity.

The particular benefit to intelligence—greater robustness, flexibility, dynamic range or better coordination—remains a hypothesis to be established independently of the scaling law.

---

# 5. Three kinds of timescale, operating concurrently

A coherent theory needs to distinguish three different temporal concepts.

**Processing/relaxation timescale $\tau_j$:** How quickly a module integrates information, reacts or relaxes after perturbation.

**Predictive horizon $h_j$:** How far into the future a representation describes reachable states or consequences.

**Learning/developmental timescale $T_j^{\mathrm{learn}}$:** How quickly the module's parameters, knowledge or structure change with experience.

A brief neural computation can retrieve a long-horizon plan; a slow neural fluctuation need not encode a distant future. The three are not interchangeable.

| Functional process | Illustrative interval | Role within a single or repeated G-loop |
|---|---|---|
| Neural signalling | Milliseconds | Local transmission and recurrent interactions |
| Perception, gating, response selection | Tens–hundreds of milliseconds | Rapid evidence selection and execution |
| Working-memory and relational coordination | Seconds | Binding, updating and maintaining intermediate structures |
| Novel synthesis and strategic switching | Seconds–minutes | Generate, constrain, infer, decide, reopen |
| Fast skill/policy banking | Sessions–weeks | Increasingly reusable procedures and control policies |
| Slow gist/schema integration | Days–months | Accumulated invariants and changed representational geometry |
| Developmental or structural change | Months–years | Altered habitual regulation, capacity interactions and network organisation |
| Niche restructuring | Variable, from a single action to years | Changes in feedback, affordances and future learning conditions |

These intervals overlap; learning and consolidation can begin during an episode, and fast neural plasticity need not wait for a later discrete phase.

## Cortical evidence for temporal hierarchy

Murray et al. (2014) measured **spiking autocorrelation timescales** across nonhuman-primate cortical regions and found shorter intrinsic timescales in sensory cortex and longer ones in prefrontal cortex. Nee (2021) independently related frontoparietal control gradients to the distinction between immediate sensory-motor demands, contextual rules and internally maintained future plans in two human fMRI samples. These results support differentiation in temporal integration and control *demands*, but not a fixed correspondence between a named network and an SR predictive horizon.

Li, Li and Wang (2025) analysed marmoset ECoG temporal organisation and fitted a multi-region model constrained by electrophysiology and anatomy. The model reproduced a hierarchy of time constants and found that near-critical model dynamics jointly favoured local integration and reliable inter-regional signal propagation. This is a particularly relevant **computational bridge**, but it is not evidence for a specifically human Griffiths phase or for Trident-G's invariant-learning operator.

The theory's stronger claim—that Gf uses the temporally differentiated hierarchy to coordinate multiple predictive horizons and learn transferable temporal invariants—is **testable rather than established**. Neural timescale estimates from spike trains, BOLD fluctuations and behavioural duration should not be treated as interchangeable. Also, the timescale-rich relaxation of a Griffiths phase is a statistical dynamical property and must be distinguished from the conventional temporal hierarchy.

## 5.1 Cross-timescale coupling

Fast learned modules provide useful building blocks for intermediate predictive maps. Intermediate maps enable Gf to infer new relations and paths. Slower schemas constrain what is relevant and which future states are worth considering. Unexpected evidence can travel upwards, while goals and prior knowledge influence which lower-level processes are recruited.

In successor-representation (SR) notation, a discounted predictive map for a suitable transition matrix $P$ is:

$$
SR_{\beta}=(I-\beta P)^{-1},\qquad 0\leq\beta<1.
$$

Different discounts $\beta$ provide different effective predictive horizons. The map's horizon is **not** the physical decay time of the module performing the computation.

The Gf synthesis process may integrate several SR horizons with current relational and generative representations. This supplies a route for learning *temporal invariants*: relationships that generalise not only across surface contexts but also across appropriately transformed sequences, delays or future horizons.

## 5.2 Learning changes temporal organisation

A working hypothesis is that repeated, validated execution changes the computational hierarchy itself:

$$
\dot\tau_j=\mathcal T_j(\tau_j,K^{Gc}_j,\mathbf p_j,W,\mathbf z),
\qquad
\dot W=\mu\,\mathcal U(W,\mathbf y,\mathbf a,\text{feedback}),
$$

where $\mathbf p_j$ records practice and $\mu$ denotes comparatively slow structural updating. These are **open developmental functions**; there is no assumed universal rule that all learning shortens $\tau_j$.

Learning can make a lower-level routine faster or more autonomous while enabling *higher-level* integration over longer predictive horizons. It can therefore sharpen temporal differentiation while improving selective coordination.

---

# 6. The four Gf computational branches and their synthesis

The entropy–mutual-information distinction is crossed with an internal–external distinction.

## 6.1 FPCN-A and FPCN-B: an empirically grounded internal–external substrate

**This is the principal candidate neural substrate for Trident-G's internal/external processing axis.** Human network-neuroscience findings support *preferential*, but not exclusive, differentiation within the frontoparietal control network (FPCN):

| System | Relatively stronger network coupling | Functions supported in the empirical literature | Specific Trident-G interpretation |
|---|---|---|---|
| **FPCN-A** | **Default network (DN/DMN)** | Introspective or internally oriented control; abstract/relational thinking, mentalising, prospective cognition | Candidate control interface for **internal** representations, long-term working-memory retrieval and predictive models |
| **FPCN-B** | **Dorsal attention network (DAN)** | Control of externally directed attention, relevant sensory/task information and action-related demands | Candidate control interface for **external** evidence selection, perceptual task rules and short-term working-memory engagement |
| **FPCN-A ↔ FPCN-B** | Reciprocal within-FPCN interactions, which vary across tasks | Linking self-generated/internal content with externally anchored attention and response | Candidate integrative route for transfer from internal models to external constraint testing and action |

**Foundational fractionation evidence.** Dixon et al. (2018) classified FPCN activity/connectivity across **four independent datasets and nine conditions**, finding that FPCN-A couples preferentially with DN and FPCN-B with DAN. Meta-analytic functional profiling favoured mentalising/emotion for A and perceptual attention/action for B. Importantly, both were associated with executive functions, and their connectivity changed by task: they are neither isolated nor exclusive circuits. Earlier network analysis by Spreng et al. (2013) established that control-network coupling can mediate interactions between default and dorsal-attention systems. Later experiments by Yin, Li and Chen (2022) demonstrated task-related **DN → FPCN-A → FPCN-B → DAN** bridging when self-referential processing aided visual working memory.

**Convergent whole-network evidence.** Murphy et al. (2020) studied working-memory network dynamics in **644 participants**, finding two frontoparietal subnetworks preferentially coupled with DN or DAN, with structural/functional coupling associated with working-memory ability; their coupled-oscillator model offers a useful precedent for the proposed $W_{jk}$ interactions. Nee (2021) characterised an **external/present → internal/future** frontoparietal gradient, with an intermediate integration zone whose dynamics predicted aspects of cognitive ability. Cole et al. (2013) found task-dependent brain-wide reconfiguration of frontoparietal connectivity. Together, these studies support task-sensitive differentiation and flexible integration rather than an anatomically fixed two-box executive system.

**An explicit boundary between evidence and interpretation.** The evidence supports the **internal/external preference**, not the stronger assertion that **FPCN-A uniquely implements long-term working memory (LT-WM) or abstract successor representations**, or that **FPCN-B uniquely implements short-term working memory (ST-WM)**. Those are Trident-G's proposed *functional specialisations*, subject to competition from other neural accounts and to the fact that both networks participate in working-memory control. Neither region is an exclusive source of Gf or Gc.

### 6.1.1 Two orthogonal axes, not a one-to-one neurochemical mapping

In the **May 2026 Trident-G formulation**, the FPCN-B side was also associated with the **entropy arm**, while FPCN-A was associated with the **mutual-information constraint arm**. Those are useful functional predictions about *typical recruitment under certain tasks*, but they should **not be presented as direct identities**, given evidence that internal and external cognition each need both exploration and evidence constraint.

The unified November formulation therefore treats the axes separately:

| | **Entropy-oriented search** | **Mutual-information-oriented constraint** |
|---|---|---|
| **Internal** — preferential FPCN-A↔DMN interface | Generate hypotheses, counterfactuals and model recombinations | Infer/compare internal relations, constraint-check candidate models |
| **External** — preferential FPCN-B↔DAN interface | Sample new cues, experiment and search environmental affordances | Select reliable evidence, update task rules and test predictions |

Both frontoparietal subsystems can contribute to both information-processing modes. Hippocampal/entorhinal and orbitofrontal representations may supply structured predictive maps; salience/interoceptive and striatal dopaminergic systems may influence *which* process is recruited. These are distributed interactions, not a four-module anatomical atlas.

The corresponding **neural-to-computational mapping** is deliberately an *estimated operator*, not an identification:

$$
\boxed{
\mathbf b_t\approx\mathcal R_{\mathrm{neuro}}\!
\left(\mathbf n_{A,t},\mathbf n_{B,t},
\mathbf n_{DMN,t},\mathbf n_{DAN,t},
\mathbf n_{HPC,t},\mathbf o_t;\Theta\right).
}
$$

Here $\mathbf n$ denotes independently measured network states and $\Theta$ task- and individual-dependent parameters. The unknown function $\mathcal R_{\mathrm{neuro}}$ **must** be fitted and validated; neither functional connectivity nor BOLD amplitude equals entropy, mutual information or a latent Trident capacity.

**Direct falsification strategy.** Manipulate *internal vs external* representational context orthogonally to *open search vs diagnostic constraint* in a factorial task. Predict FPCN-A↔DMN versus FPCN-B↔DAN differences principally by the **context axis**, and differences in search/constraint processing principally by the **computational axis and their interactions**, with task-dependent within-FPCN bridging. Test whether network measures predict behaviour beyond task difficulty, arousal, working-memory demand and domain knowledge. If the 2 × 2 dissociation does not appear, revise the neural mapping without redefining the psychological operations.



## 6.2 Computational branches, synthesis and learning

| Branch | Computational emphasis | Typical contribution |
|---|---|---|
| **Internal × entropy-oriented** | Generative exploration | Hypotheses, counterfactuals, recombinations, model variation |
| **Internal × mutual-information-oriented** | Relational inference | Structure mapping, abstraction, evaluation of internal relationships |
| **External × entropy-oriented** | Environmental search | Testing, sampling, intervention and discovery of affordances |
| **External × mutual-information-oriented** | Evidence constraint | Diagnostic sampling, prediction-error evaluation, task-relevant relationships |

Entropy and mutual information are information-theoretic quantities, **not independent anatomical subsystems or opposite critical phases**. Each branch denotes a proposed mode of computation. The hypothesis that FPCN subdivisions, dorsal-attention, default-mode and hippocampal systems contribute differentially is testable, not an identity built into the equations.

Let the active branches form $\mathbf b_t=(b_{IE},b_{IM},b_{EE},b_{EM})^\top$, with first index internal/external and second index entropy/mutual-information. Their interactions can be written:

$$
d\mathbf b_t=\mathbf F_b(\mathbf b_t,\mathbf y_t,\mathbf o_t,
K_t^{Gc},\mathbf c_t,\mathbf z_t,\boldsymbol\zeta_t)\,dt
+\Sigma_b\,d\mathbf W_t^{(b)}.
$$

Gf synthesis combines these modes with retrieved skills, background schemas and predictive maps:

$$
\boxed{
\mathbf r_t^\star=
\mathcal S\Big(
\mathbf b_t,\{\gamma_{j,t}Q_jy_{j,t}\}_j,
K_t^{Gc},\{SR_{\beta_h}\}_h,\mathbf o_t,\mathbf z_t
\Big).
}
$$

Here $\mathbf r_t^\star$ is the active, synthesised representation: potentially a causal model, relational hypothesis, problem-solving plan or strategy. $Q_j$ translates specialised module outputs into a usable common representation. The explicit computational form of $\mathcal S$ is **not yet specified**; it is a central research target.

### Neural evidence for combining generated and goal-constrained representations

Functional interactions among DMN, executive-control and salience-associated regions have been observed during creative cognition. In particular, Beaty et al. (2018) identified connectivity patterns linking these systems that predicted individual divergent-thinking performance across samples. This lends support to **network cooperation between spontaneous generation and controlled evaluation**, without showing that DMN computes Shannon entropy, that FPCN computes mutual information, or that such coupling equals psychometric Gf.

The FPCN internal–external distinction is best treated as a *routing or representational-context preference*, whereas entropy-oriented search and relevance-oriented constraint are proposed **computational operations**. Their crossed 2 × 2 structure is the Trident-G hypothesis to be tested within the same factorial task, not four validated anatomical pathways.

### Why Gf might predict invariant learning

The theory predicts that higher independently measured Gf will, under suitable conditions, be associated with better discovery and coordination of relational structures across transformations and predictive horizons. This is **not** the same as claiming that Gf training necessarily raises invariant-learning ability or causes far transfer. Existing Gc, working-memory capacity, task demands, feedback and prior knowledge are relevant competing predictors.

A strong test must measure Gf independently, systematically vary relational complexity and transformations, and assess genuinely held-out and delayed applications.

---

# 7. From local success to transferable invariants

A novel solution is not automatically a portable invariant. An invariant is a relation preserved under a **specified family of relevant transformations**. The family might alter surface features, response mappings, context, temporal spacing, or niche while retaining the causal/relational structure needed for the task.

For representation $r_\theta$ and structure-preserving transformation $T$:

$$
r_\theta(TX)\approx r_\theta(X).
$$

Some tasks require *equivariance* rather than invariance—i.e. $r_\theta(TX)\approx\rho(T)r_\theta(X)$—where the representation transforms predictably instead of remaining literally unchanged.

A constant representation would satisfy simple invariance but convey no useful information. Therefore, the proposed learner must retain **predictive or action-relevant sufficiency**. One illustrative objective is:

$$
\mathcal L_{\mathrm{inv}}(\theta)
=
\mathbb E_{X,T}\|r_\theta(TX)-r_\theta(X)\|^2
+\beta\,\mathbb E_{X,Y}\ell\big(\widehat Y(r_\theta(X)),Y\big),
$$

subject to transformations genuinely preserving the target relationship. Other implementations may use relational graphs, structured causal models or SR mappings rather than vectors.

Let $\mathbf q_t$ be the developing invariant representation and $v_t\in[0,1]$ a validation weight reflecting evidence from variation, near-miss cases, real use and delay:

$$
\dot{\mathbf q}_t=
\mathcal M(\mathbf q_t,\mathbf r_t^\star,
\mathbf o_t,\mathbf a_t,\mathbf z_t,\mathcal D_{\leq t}).
$$

The function $\mathcal M$ is a candidate invariant-learning mechanism, **not yet an executable estimator**.

The proposed transfer criterion includes both **horizontal transfer** (structure survives changed wrappers or niches) and **vertical transfer** (the adaptive policy can be reconstructed across attention, binding, prediction, inference and action). Delayed recovery is required to distinguish durable learning from transient task priming.

---

## Empirical substrate for relational maps and predictive inference

The hippocampal–entorhinal system offers a plausible source of structured relational representations, though not a direct proof of the full Trident synthesis operator. **Garvert, Dolan and Behrens (2017)** used human fMRI adaptation to identify abstract, nonspatial relational maps whose distances tracked associative and future-state structure. **Schuck et al. (2016)** decoded partially hidden task states from human orbitofrontal cortex; decoding quality related to decision behaviour. **Momennejad et al. (2017)** found behavioural evidence for successor-representation-like choice in two human studies, separating sensitivity to reward changes from sensitivity to transition changes. **Stachenfeld, Botvinick and Gershman (2017)** formalised the hippocampus as a predictive map using computational modelling.

**Interpretation.** These converging results support the possibility of relational, state-space and SR-like representations used during planning. They do not demonstrate that FPCN-A alone performs LT-WM or that all relational invariants are represented as SRs. The model should test whether changed-format transfer is explained by learned relational *structure*, not merely by familiarity with a broad class of inputs.

# 8. Gf→Gc→Gf banking builds both knowledge and modules

Consolidation has at least two related outputs.

**Fast Gc compilation** produces readily available procedures, local control policies, task rules and skilled subroutines. Some may become relatively autonomous and recruitable as modules.

**Slow Gc integration** produces gist, general relational schemas and representational organisation accumulated across episodes. This can reshape which variables, constraints and connections are salient during later Gf search.

These are functional pathways and different characteristic learning timescales, not assertions that each can be assigned to a single isolated anatomical site.

**Neural evidence and boundaries.** Vatansever, Menon and Stamatakis (2017) found increased DMN engagement during automated rule use in predictable conditions, including task-related interactions with hippocampal/parahippocampal regions. This supports a memory-based automated mode but **does not identify all Gc with the DMN**. Tse et al. (2007, 2011) used rat schema-learning experiments to show that pre-existing knowledge can strongly accelerate integration of new associations, with a critical contribution from medial prefrontal circuitry. These studies support schema-dependent consolidation, but not the specific fast/subcortical versus slow/cortical partition proposed here.

A July 2026 **non-peer-reviewed preprint** by Xue et al. reported lower intracellular neuronal glucose consumption per task after learning in behaving mice. If replicated, this is useful evidence for learning-related task efficiency; it is **not** evidence that Gc has a specific neural criticality sign or that human Gc retrieval generally consumes less total energy than Gf reasoning.

Let $K_t^f$ and $K_t^s$ denote fast and slow Gc stores. A schematic distinction is:

$$
\begin{aligned}
\dot K_t^f &=
\rho_f v_t\mathcal B_f(\mathbf q_t,\mathbf r_t^\star,\text{feedback})
-\Gamma_f(K_t^f),\\
\dot K_t^s &=
\rho_s\mathcal B_s(K_t^s,\mathcal D_{\leq t},K_{\leq t}^f,\text{rest})
-\Gamma_s(K_t^s).
\end{aligned}
$$

The second equation allows across-episode consolidation, including sleep/rest-dependent effects, without asserting that all slow Gc construction requires a single fixed interval. The model should avoid banking a policy merely because it is fluent or immediately rewarding. The candidate must have defensible boundary conditions and sufficient evidence of portability.

The developmental cycle is therefore:

**Gf opens and synthesises → action tests a candidate relation → invariant validation → fast Gc modules and slower Gc schemas → more efficient or better-structured future Gf.**

This is a *spiral* only when the new structures alter later reachable problems, learning trajectories or representations. Repeating the same task more fluently without broader structural change may be successful training but is not sufficient evidence for general intelligence growth.

---

# 9. Capacity mutualism and developmental change

Let the four Trident capacities be

$$
\mathbf c_t=(c_F,c_R,c_E,c_L)^\top.
$$

Their development depends on practice, available knowledge, current branch coordination, niche opportunities and possible interactions:

$$
\boxed{
\dot c_{i,t}=
L_i(c_i,\mathbf p_i,K_t^f,K_t^s,\mathbf z_t)
+\sum_{j\ne i}w_{ij}\,M_{ij}(\mathbf c_t,\mathbf b_t,\mathbf z_t).
}
$$

The weights need not be symmetric: $w_{ij}\ne w_{ji}$. A gain in one function could alter the *subsequent rate or depth* at which another function can be learned. This is a stronger form of developmental mutualism than a contemporaneous correlation among ability scores.

The empirical challenge is to distinguish such a causal effect on later learning from ordinary shared variance, practice, strategic knowledge and test overlap. Network centrality does not automatically imply intervention leverage. The model must permit zero or even negative transfer where evidence warrants it.

---

## Neuroplasticity and asymmetric learning opportunities

Evidence that network organisation changes with learning (Bassett et al., 2011) and that frontoparietal integration relates to higher-level control (Cole et al., 2013; Nee, 2021) makes a developmental network account biologically plausible. However, none of these studies directly demonstrates that training one Trident capacity *causally increases the future learning rate* of another. That stronger asymmetric-mutualism claim requires longitudinal, intervention-based analysis, not resting-state covariance or network centrality alone.

# 10. Coupled niches and the regulation of future possibilities

An individual operates within several partly connected niches: work, research, social relationships, educational settings, AI-mediated workflows, and others. An adaptive policy can be effective only when the niche provides relevant cues, authority, affordances and feedback.

Let $\mathbf z_{n,t}$ represent niche $n$. A general reciprocal model is:

$$
\boxed{
\dot{\mathbf z}_{n,t}
=f_n(\mathbf z_{n,t})
+\sum_{m\ne n}H_{nm}(\mathbf z_{m,t},\mathbf z_{n,t})
+B_n\mathbf a_t.
}
$$

Niches influence cognition through $\lambda_{n,t}$ and observational feedback; action changes niches through $B_n\mathbf a_t$. Niche coupling is therefore not merely context in which an internal skill happens to be tested: the environment may enable, distort, block or transform the policy itself.

Niche-specific knowledge can draw upon direct experience, consolidated Gc and cross-niche mappings:

$$
\dot K_{n,t}=
\mathcal L_n(K_{n,t},\mathbf o_t,\mathbf a_t)
+\nu_n\mathcal T_n(K_t^{Gc})
+\sum_{m\ne n}\nu_{mn}\mathcal T_{mn}(K_{m,t}).
$$

The mappings $\mathcal T_{mn}$ should preserve relevant structure; their existence and effectiveness must be *demonstrated*, not presumed.

### Neural grounding versus external-niche evidence

The allostatic–interoceptive evidence (Kleckner et al., 2017; Zhang et al., 2025) supports the claim that internal physiological regulation and broad cognitive systems are integrated. It does **not** by itself demonstrate that changing a workplace, educational system or social niche produces general-intelligence gains. Niche construction is consequently a computational/behavioural extension that requires its *own* intervention and transfer evidence, with changes in environmental affordances and feedback measured independently from brain activity.

### Adaptation, growth and viable control

Immediate adaptation means meeting current demands while maintaining viable regulation. Growth is a stronger claim: learning and action expand the set of **future states and niches in which the agent can act effectively**.

Let $\mathcal V$ be a viable range of regulatory conditions, and $\Omega_t$ a suitably defined set of future controllable possibilities. A candidate control objective can reward immediate personally valued outcomes, costs, successful adaptation and change in $\Omega_t$, subject to viability constraints:

$$
J(\pi)=\mathbb E_\pi\!\left[
\sum_{t=0}^T \gamma^t
\left(R_t-C_t+\alpha A_t+\beta\Delta\Omega_t\right)
\right],
\qquad
\Pr_\pi(\mathbf h_t\in\mathcal V\ \forall t)\geq 1-\rho.
$$

This is an illustrative normative objective, not a validated metric of intelligence. The weights, values, time horizon and acceptable risks cannot be inferred from neural criticality. Their specification is part of the agent's purposes and social setting.

The theory accordingly separates **robustness** (remaining viable and recovering after disturbance), **flexibility** (accessing diverse appropriate processes and policies) and **growth** (changing the repertoire of future effective actions).

---

# 11. A unified intelligent episode: the G-loop

The G-loop is best understood as a **concurrent, recursively updating process**, not a rigid serial programme.

An episode can be described as follows. The agent enters a viable state; multiple automated skills remain active; observations and familiar knowledge constrain a novel problem; Gf explores and integrates alternatives; meta-control decides when more evidence is valuable and when action is warranted; the action alters the niche; its consequences generate prediction errors; local processes are adjusted or higher-level search is reopened; useful relational structures are validated against transformations; fast and slow Gc banking changes what will be available next time.

This involves two simultaneously operating feedback circuits:

**Within-episode regulation:** state → recruitment and synthesis → action → feedback → targeted correction or switching.

**Across-episode development:** tested solutions → transferable invariants → skill/schema banking → changed modules, timescales and predictive maps → altered future episodes and niches.

A high-Gf episode is not one in which every module is constantly near-critical or consciously controlled. It is one in which the system can **selectively combine existing competence with flexible reconstruction** under the present demands.

---

# 12. Testable predictions and discriminating experiments

The strongest predictions must distinguish Trident-G from simpler accounts. The following are hypotheses; none follows automatically from the use of mathematical notation.

| Candidate prediction | Operational test | Important comparison or control |
|---|---|---|
| **P1. Hysteretic strategy change** | Slowly sweep uncertainty, effort and reward contingencies; fit switching thresholds and return paths | Smooth RL, hidden-state and non-cusp nonlinear models |
| **P2. Concurrent Gc/Gf coordination** | Train several routines, then test unfamiliar compositions while measuring local routine preservation and higher-level coordination | Independent routine execution; flat control and standard hierarchical RL |
| **P3. Extended critical-like operating range adds value** | Simulate matched modular networks with and without rare-region/Griffiths dynamics across task/load parameters | Degree-, hierarchy-, resource- and performance-matched noncritical controls |
| **P4. Gf predicts invariant learning** | Independent Gf testing; vary surface and structural transformations, hold out transfer tasks and test after delay | Gc, working memory, processing speed and initial task learning |
| **P5. Gf predicts temporal-horizon coordination** | Require recombination of short-, medium- and long-horizon predictive relationships | Speed, working memory, established Gc and baseline graph-learning ability |
| **P6. Fast and slow banking dissociate** | Compare immediate fluency, automatic execution, delayed schema transfer and rest/consolidation conditions | Exposure, repetition, strategy instruction and baseline knowledge |
| **P7. Niche construction changes later adaptability** | Give some agents the ability to change workflow or feedback structure; compare future reachable tasks and resilience | Same immediate reward, experience and task difficulty without niche control |
| **P8. Signed prediction errors modulate tilt without dictating exploration** | Manipulate better-than-expected, expected and worse-than-expected outcomes orthogonally to expected information gain; estimate subsequent policy persistence, switching and novel search | Compare RPE-only, uncertainty-only and combined gated-RPE/epistemic models; distinguish local avoidance from generative exploration |
| **P9. Internal/external frontoparietal substrate** | Factorially vary internal versus externally anchored processing and open search versus diagnostic constraint; estimate FPCN-A–DMN and FPCN-B–DAN coupling and FPCN-A↔B interactions | Control relational complexity, Gf, working-memory difficulty, visual input and arousal; compare separate-axes model with original FPCN-A=MI/FPCN-B=entropy identity |
| **P10. Allostatic network involvement in regulatory recovery** | Combine brain network, pupil/autonomic and behavioural time series after controlled challenge and recovery | Test multimodal gain beyond single biomarkers and generic arousal; avoid inferring $F^\star$ directly from one physiological channel |
| **P11. Neural modularity predicts novel composition** | Repeatedly measure connector-network reconfiguration during unfamiliar combinations of trained skills | Compare specialist routine accuracy, hierarchical RL, and familiarity; test generalisation beyond trained component sequences |

### What specifically counts as evidence for a Griffiths phase?

Not just $1/f$ spectra, heavy-tailed reaction times or individual neuronal avalanches. The network hypothesis requires an appropriate dynamical model and convergent evidence for **an extended parameter interval** with scale-rich relaxation, localised persistence or related signatures. Analyses should test finite-size effects, nonstationarity, fitting range, alternative heavy-tail generators and robustness to different inference methods.

### What counts as evidence for higher *general* intelligence?

Improvements must extend beyond the trained tasks and surface similarities, survive delay and demonstrate predictive value for unfamiliar problems. If a hierarchical controller explains all the behavioural benefits without a Griffiths-phase regime, the **hierarchy** remains useful but the **criticality-specific** claim is not supported.

---

# 13. Implementation priorities and identification limits

The fully coupled model contains more latent states than could responsibly be inferred from a short behavioural session. It is therefore best developed in stages.

**First: minimal behavioural controller.** Implement the cusp with measured or manipulated task demands, a small bank of learned policies, one flexible synthesis operation, and simple feedback. Test whether the cusp improves held-out prediction of switching or resilience beyond non-cusp competitors.

**Second: hierarchical modular learner.** Add gated skill modules and an independently manipulable network topology. Compare successful novel compositions against a flat agent and ordinary hierarchical reinforcement learning.

**Third: multiscale and criticality tests.** Introduce explicit local propagation rules and heterogeneity, then establish whether a Griffiths-like interval *emerges* and produces advantages beyond hierarchy alone. Distinguish $\tau_j$ from predictive SR horizons.

**Fourth: invariant learning and Gc banking.** Implement meaningful structure-preserving transformations, validated transfer mappings, fast policy compilation and slower schema integration. Test both immediate composition and delayed recovery.

**Fifth: reciprocal niches and human validation.** Extend agents to modifiable environments, then fit targeted human tasks with independent Gf/Gc measures, appropriate repeated assessments, and cautiously interpreted neural/physiological signals.

The earliest computational implementation should **freeze slow developmental variables** and specify concrete forms for $\mathcal S$, $\mathcal M$, $\mathcal A$, $\mathrm{Gate}$, $f_j$ and $\mathcal B$. Meta-efficacy $\eta$, coherence $\chi$, homeostatic conditions $\mathbf h$, and $F^\star$ presently enter as inputs or slow latent quantities: their own update laws are open questions. Version 0.3 is therefore a *structured candidate theory*, not yet a closed, identifiable model.

---

# Appendix A. Compact mathematical framework (v0.3)

The equations below are the minimal mutually consistent **schema**, not yet a numerical specification. Unless otherwise noted, all variables are time-dependent. $\mathbf W$ denotes Wiener noise and $W_{jk}$ denotes network weights; these are different symbols.

**A1. Original Trident state and allostatic mismatch**

$$
x=F-F^\star,\qquad \xi=G-F^\star,\qquad \varepsilon=F-G.
$$

**A2. Cusp potential and mesoscopic state dynamics**

$$
V(x;\xi,\delta)=x^4-\xi x^2-\delta x,\qquad
dx=(-4x^3+2\xi x+\delta)\,dt+\sigma_x\,dW^{(x)}.
$$

**A3. Anticipated load, signed RPE learning and exploration–exploitation tilt**

$$
\begin{aligned}
G&=\mathscr G(\mathbf c,\eta,\chi,\mathbf h,K^{Gc},\mathbf b,\mathbf z,\text{goal}),\\
\Delta_t^R&=r_t-\widehat r_t,\quad
\ell_t^{+}=\alpha_{+}[\Delta_t^R]_{+},\quad
\ell_t^{-}=\alpha_{-}[-\Delta_t^R]_{+},\\
\delta_t^{\mathrm{base}}&=u_t+\sum_n\lambda_{n,t}\psi_n(\mathbf z_{n,t},K_{n,t})
+\boldsymbol\omega^\top\mathbf b_t,\\
\delta_{t+1}&=\mathrm{clip}\big[
\rho_\delta\delta_t+(1-\rho_\delta)\delta_t^{\mathrm{base}}
+\beta_+g_t^+\ell_t^+-\beta_-g_t^-\ell_t^-
+\beta_C S_t-\beta_E\mathrm{EIG}_t
\big].
\end{aligned}
$$

$\Delta^R$ is a reward error, not the allostatic $\varepsilon=F-G$; $\ell^-$ models *learning consequences of dopamine decreases/indirect-pathway disinhibition*, not increased D2 receptor activation. A negative RPE weakens the old policy only where context warrants it; whether wider exploration follows is a **separate** choice.

**A4. Hierarchical modular dynamics**

$$
\tau_j\,dy_j=
\left[f_j(y_j;K_j^{Gc},\zeta_j)+\sum_kW_{jk}H_{jk}(y_k,y_j)
+\gamma_jB_j\mathbf r^\star_{t^-}+I_j\right]dt+\sigma_j\,dW^{(j)}.
$$

**A5. Local criticality, distinguishable from cusp control**

$$
\zeta_j=m_j-1,\qquad
\dot\zeta_j=-\rho_j(\zeta_j-\zeta_j^\star(\text{task},\mathbf h,\mathbf z))+\nu_j.
$$

The $\zeta_j$ equation is an optional regulatory hypothesis, not a demonstrated biological controller.

**A6. Branch processes and synthesis**

$$
d\mathbf b=\mathbf F_b(\mathbf b,\mathbf y,\mathbf o,K^{Gc},
\mathbf c,\mathbf z,\boldsymbol\zeta)\,dt+\Sigma_b\,d\mathbf W^{(b)},
$$

$$
\mathbf r^\star=\mathcal S\left(\mathbf b,
\{\gamma_jQ_jy_j\}_j,K^{Gc},
\{SR_{\beta_h}\}_h,\mathbf o,\mathbf z\right).
$$

**A6b. Candidate network-to-computation mapping (to be estimated)**

$$
\mathbf b_t\approx
\mathcal R_{\mathrm{neuro}}
(\mathbf n_{A,t},\mathbf n_{B,t},
\mathbf n_{DMN,t},\mathbf n_{DAN,t},
\mathbf n_{HPC,t},\mathbf o_t;\Theta).
$$

Dixon et al.'s FPCN-A/DMN versus FPCN-B/DAN **preferential coupling** motivates the internal–external axis, while entropy/MI-oriented modes remain distinct, orthogonal computational hypotheses. A shared latent signal should not be counted as an independently validated neural measure of $b_{IE}$, $b_{IM}$, $b_{EE}$ or $b_{EM}$.

**A7. Skill gating and assembled action**

$$
\gamma_j=\mathrm{Gate}_j(\mathbf o_{t^-},\mathbf r^\star_{t^-},e_{j,t^-},\mathbf z,\eta),\qquad
\mathbf a=\mathcal A\left(\mathbf a^{Gf},\{\gamma_j\pi_j^{Gc}\}_j\right).
$$

**A8. Candidate invariants and dual Gc banking**

$$
\begin{aligned}
\dot{\mathbf q}&=\mathcal M(\mathbf q,\mathbf r^\star,\mathbf o,\mathbf a,\mathbf z,\mathcal D_{\le t}),\\
\dot K^f&=\rho_fv\,\mathcal B_f(\mathbf q,\mathbf r^\star,\text{feedback})-\Gamma_f(K^f),\\
\dot K^s&=\rho_s\mathcal B_s(K^s,\mathcal D_{\le t},K^f_{\le t},\text{rest})-\Gamma_s(K^s).
\end{aligned}
$$

**A9. Capacity mutualism and slow structural adaptation**

$$
\dot c_i=L_i(c_i,\mathbf p_i,K^f,K^s,\mathbf z)
+\sum_{j\ne i}w_{ij}M_{ij}(\mathbf c,\mathbf b,\mathbf z),
$$

$$
\dot\tau_j=\mathcal T_j(\tau_j,K_j^{Gc},\mathbf p_j,W,\mathbf z),
\qquad \dot W=\mu\mathcal U(W,\mathbf y,\mathbf a,\text{feedback}).
$$

**A10. Niche change and cross-niche learning**

$$
\dot{\mathbf z}_n=f_n(\mathbf z_n)
+\sum_{m\ne n}H_{nm}(\mathbf z_m,\mathbf z_n)+B_n\mathbf a,
$$

$$
\dot K_n=\mathcal L_n(K_n,\mathbf o,\mathbf a)
+\nu_n\mathcal T_n(K^{Gc})
+\sum_{m\ne n}\nu_{mn}\mathcal T_{mn}(K_m).
$$

**A11. Strategic control**

$$
(\mathbf a^{Gf},u)=
\pi(x,\mathbf c,K^f,K^s,\mathbf r^\star,\eta,\chi,\mathbf z).
$$

Operational decisions should be implemented on an explicit sampling/update schedule or as a specified coupled stochastic system to avoid algebraic circularity. The symbolic operators above cannot be fitted without defining compatible state spaces and observations.

## Appendix B. Notation and crucial distinctions

| Quantity | Interpretation |
|---|---|
| $x=F-F^\star$ | Realised deviation from defended homeostatic reference |
| $\xi=G-F^\star$ | Anticipated engagement relative to defended reference; cusp shape control |
| $\varepsilon=F-G$ | Allostatic realised-versus-expected mismatch |
| $\delta$ | Explore–exploit/convergent–divergent tilt |
| $\zeta_j=m_j-1$ | Optional local propagation criticality metric; **not** $\xi$ or $\varepsilon$ |
| $\mathbf c$ | Four functional Trident capacities |
| $\mathbf b$ | Four computational entropy/MI × internal/external branches |
| $y_j,\gamma_j,W_{jk}$ | Module state, recruitment gate and network coupling |
| $\tau_j$ | Module processing/relaxation timescale |
| $h_j$ or $\beta_h$ | Predictive temporal horizon or SR discount |
| $K^f,K^s$ | Fast compiled Gc and slow schematic Gc |
| $\mathbf q,v$ | Candidate invariants and validation strength |
| $\mathbf r^\star$ | Synthesised relational/problem representation |
| $\eta,\chi$ | Meta-efficacy and coherence (latent control parameters) |
| $\lambda_n,\mathbf z_n$ | Niche coupling and niche state |
| $\mathbf a,u$ | External action and strategic internal control |

**Reward prediction error $\Delta^R$ ≠ allostatic mismatch $\varepsilon=F-G$ ≠ entropy or mutual information.**  
**Dopamine-dependent Go/NoGo learning ≠ direct biochemical implementation of strategic exploration.**  
**Cusp bifurcation ≠ local activity propagation ≠ Griffiths phase.**  
**Processing timescale $\tau$ ≠ predictive horizon $h$ ≠ learning timescale.**  
**Functional Gc automaticity ≠ proven subcritical neural activity.**  
**Complex modularity ≠ proven criticality-specific cognitive advantage.**  
**Transfer across changed tasks ≠ established increase in psychometric general intelligence.**

---

# Appendix C. Evidence boundary and research sources

### Established or independently studied building blocks

Neural avalanche and criticality phenomena; hierarchical modular and heterogeneous network models; hierarchical reinforcement-learning descriptions of learned action sequences; successor representations as predictive maps; distinct neural temporal integration windows; and broad empirical distinctions between novel reasoning, skills and accumulated knowledge.

### Theoretical interpretations requiring direct testing

That Trident-G's cusp variables track human homeostatic engagement; that the Ψ-band is an individually measurable region of adaptive near-critical operation; that Gf synthesis is specifically implemented through the stated four information-processing branches; that Gc-dominated processing preferentially recruits more subcritical and lower-cost dynamics; that a Griffiths phase causally improves Gf/Gc coordination; and that improved invariant learning produces durable, domain-general gains in intelligence.

### Evidence audit: which neural findings support which claims?

This table grades the **strength and directness of the evidence for the stated component**, not the plausibility of the whole Trident-G theory. "Direct" refers to the measured phenomenon in the cited study; it does not imply that its proposed role in Trident-G has been validated.

| Proposed component | Most informative empirical anchor | Evidence status | What remains unestablished |
|---|---|---|---|
| FPCN-A↔DN versus FPCN-B↔DAN coupling | Dixon et al. (2018), four datasets/nine conditions; Murphy et al. (2020); Yin et al. (2022) | **Strong** network differentiation and preferential coupling; functional interpretation supported by task studies | Fixed, exclusive A=LT-WM and B=ST-WM anatomy; one-to-one assignment to entropy or MI |
| Dynamic integration of internal and external control | Spreng et al. (2013); Cole et al. (2013); Nee (2021) | **Substantial** fMRI evidence for flexible control-network integration and gradients | Unique causal Gf synthesis operator or a single executive controller |
| Neural basis of allostasis/interoception | Kleckner et al. (2017); Zhang et al. (2025, 7T) | **Strong** anatomical/connectivity convergence, including subcortical/brainstem regions | Identification of the scalar $F^\star$, $\xi$ or Ψ-band directly from those circuits |
| Hierarchical modular coordination | Bertolero et al. (2015); Murphy et al. (2020); Bassett et al. (2011) | **Substantial** functional network organisation and prospective learning association | Specific Gc-module/gating implementation or causal general-intelligence advantage |
| Neural temporal hierarchy | Murray et al. (2014, spikes); Li et al. (2025, ECoG plus model) | **Strong** temporal differentiation; near-critical integration advantage chiefly **model-based** | Equating neural decay $\tau$ with the SR predictive horizon or developmental learning rate |
| Near-criticality linked to cognition | Ezaki et al. (2020); Xu et al. (2022); Müller et al. (2025) | **Promising, correlational and estimator-dependent** | That Gf is always supercritical, Gc always subcritical, or criticality is uniquely causal |
| Griffiths phase in cognition | Moretti & Muñoz (2013) and hierarchical-network models | **Mathematically/computationally motivated** | Direct demonstration of a human Griffiths phase during reasoning and its specific adaptive benefit |
| Hippocampal/entorhinal and OFC relational maps | Garvert et al. (2017); Schuck et al. (2016); Momennejad et al. (2017); Stachenfeld et al. (2017 model) | **Substantial** evidence for representational and predictive structure | That all transfer invariants are hippocampal SRs or that FPCN-A solely constructs them |
| Habitual processing and Gc consolidation | Vatansever et al. (2017); Tse et al. (2007, 2011 in rats) | **Substantial for specialised mechanisms**, cross-species constraints | Universal fast/subcortical versus slow/cortical Gc partition |
| Reduced neural fuel use after learning | Xue et al. (2026, **bioRxiv preprint**, mice) | **Preliminary**, not yet peer reviewed | A general human Gc energetic advantage or a criticality mechanism |
| D1/D2 outcome-sensitive learning | Frank et al. (2004); Shen et al. (2008); Lee et al. (2021); Kravitz et al. (2012) | **Substantial**, with known exceptions and circuit heterogeneity | Direct equivalence of D1=MI or D2=entropy, or deterministic RPE→exploration |
| Asymmetric developmental mutualism and niche-driven rise in $g$ | Network reconfiguration and allostasis provide indirect constraints | **Trident-G hypothesis** | Causal improvement in a distinct capacity's *later learning rate* and genuine far-transfer gains |

**Methodological principle:** fMRI functional connectivity, behavioural Gf/Gc scores, EEG criticality proxies, neuronal spiking, neuromodulatory activity, and subjective effort are distinct measurements. Treating them as different observations of the *same* latent control system requires a model with independently validated links. A high neural–behavioural correlation is not in itself proof of a Griffiths phase or improved intelligence.

### Neuroscience research references integrated into the theory

**FPCN-A/B differentiation, internal–external coordination, and network integration**

- **Dixon, M. L., et al. (2018).** Heterogeneity within the frontoparietal control network and its relationship to the default and dorsal attention networks. *Proceedings of the National Academy of Sciences, 115*, E1598–E1607. https://doi.org/10.1073/pnas.1715766115
- **Spreng, R. N., Sepulcre, J., Turner, G. R., Stevens, W. D., & Schacter, D. L. (2013).** Intrinsic architecture underlying the relations among the default, dorsal attention, and frontoparietal control networks of the human brain. *Journal of Cognitive Neuroscience, 25*, 74–86. https://doi.org/10.1162/jocn_a_00281
- **Murphy, A. C., Bertolero, M. A., Papadopoulos, L., Lydon-Staley, D. M., & Bassett, D. S. (2020).** Multimodal network dynamics underpinning working memory. *Nature Communications, 11*, 3035. https://doi.org/10.1038/s41467-020-15541-0
- **Nee, D. E. (2021).** Integrative frontal-parietal dynamics supporting cognitive control. *eLife, 10*, e57244. https://doi.org/10.7554/eLife.57244
- **Yin, S., Li, Y., & Chen, A. (2022).** Functional coupling between frontoparietal control subnetworks bridges the default and dorsal attention networks. *Brain Structure and Function, 227*, 2243–2260. https://doi.org/10.1007/s00429-022-02517-7
- **Cole, M. W., et al. (2013).** Multi-task connectivity reveals flexible hubs for adaptive task control. *Nature Neuroscience, 16*, 1348–1355. https://doi.org/10.1038/nn.3470
- **Bertolero, M. A., Yeo, B. T. T., & D'Esposito, M. (2015).** The modular and integrative functional architecture of the human brain. *Proceedings of the National Academy of Sciences, 112*, E6798–E6807. https://doi.org/10.1073/pnas.1510619112
- **Beaty, R. E., et al. (2018).** Robust prediction of individual creative ability from brain functional connectivity. *Proceedings of the National Academy of Sciences, 115*, 1087–1092. https://doi.org/10.1073/pnas.1713532115

**Allostatic–interoceptive circuitry**

- **Kleckner, I. R., et al. (2017).** Evidence for a large-scale brain system supporting allostasis and interoception in humans. *Nature Human Behaviour, 1*, 0069. https://doi.org/10.1038/s41562-017-0069
- **Zhang, J., et al. (2025).** Cortical and subcortical mapping of the human allostatic–interoceptive system using 7 Tesla fMRI. *Nature Neuroscience, 28*, 2380–2391. https://doi.org/10.1038/s41593-025-02087-x
- **Sridharan, D., Levitin, D. J., & Menon, V. (2008).** A critical role for the right fronto-insular cortex in switching between central-executive and default-mode networks. *Proceedings of the National Academy of Sciences, 105*, 12569–12574. https://doi.org/10.1073/pnas.0800005105

**Criticality and network dynamics, including contradictory findings**

- **Ezaki, T., et al. (2020).** Closer to critical resting-state neural dynamics in individuals with higher fluid intelligence. *Communications Biology, 3*, 52. https://doi.org/10.1038/s42003-020-0774-y
- **Xu, L., Feng, J., & Yu, L. (2022).** Avalanche criticality in individuals, fluid intelligence, and working memory. *Human Brain Mapping, 43*, 2534–2553. https://doi.org/10.1002/hbm.25802
- **Liu, X., Fei, X., & Liu, J. (2025; online 2024).** The cognitive critical brain: Modulation of criticality in perception-related cortical regions. *NeuroImage, 305*, 120964. https://doi.org/10.1016/j.neuroimage.2024.120964
- **Müller, P. M., Miron, G., Holtkamp, M., & Meisel, C. (2025).** Critical dynamics predicts cognitive performance and provides a common framework for heterogeneous mechanisms impacting cognition. *Proceedings of the National Academy of Sciences, 122*, e2417117122. https://doi.org/10.1073/pnas.2417117122
- **Priesemann, V., et al. (2014).** Spike avalanches in vivo suggest a driven, slightly subcritical brain state. *Frontiers in Systems Neuroscience, 8*, 108. https://doi.org/10.3389/fnsys.2014.00108

**Temporal processing, knowledge learning and consolidation**

- **Murray, J. D., et al. (2014).** A hierarchy of intrinsic timescales across primate cortex. *Nature Neuroscience, 17*, 1661–1663. https://doi.org/10.1038/nn.3862
- **Li, G., Li, S., & Wang, X.-J. (2025).** A hierarchy of time constants and reliable signal propagation in the marmoset cerebral cortex. *Nature Communications, 16*, 11640. https://doi.org/10.1038/s41467-025-66699-4
- **Bassett, D. S., et al. (2011).** Dynamic reconfiguration of human brain networks during learning. *Proceedings of the National Academy of Sciences, 108*, 7641–7646. https://doi.org/10.1073/pnas.1018985108
- **Garvert, M. M., Dolan, R. J., & Behrens, T. E. J. (2017).** A map of abstract relational knowledge in the human hippocampal–entorhinal cortex. *eLife, 6*, e17086. https://doi.org/10.7554/eLife.17086
- **Schuck, N. W., Cai, M. B., Wilson, R. C., & Niv, Y. (2016).** Human orbitofrontal cortex represents a cognitive map of state space. *Neuron, 91*, 1402–1412. https://doi.org/10.1016/j.neuron.2016.08.019
- **Momennejad, I., et al. (2017).** The successor representation in human reinforcement learning. *Nature Human Behaviour, 1*, 680–692. https://doi.org/10.1038/s41562-017-0180-8
- **Vatansever, D., Menon, D. K., & Stamatakis, E. A. (2017).** Default mode contributions to automated information processing. *Proceedings of the National Academy of Sciences, 114*, 12821–12826. https://doi.org/10.1073/pnas.1710521114
- **Tse, D., et al. (2007).** Schemas and memory consolidation. *Science, 316*, 76–82. https://doi.org/10.1126/science.1135935
- **Tse, D., et al. (2011).** Schema-dependent gene activation and memory encoding in neocortex. *Science, 333*, 891–895. https://doi.org/10.1126/science.1205274
- **Xue, K., et al. (2026).** Learning shapes the energy cost of neural tasks. *bioRxiv preprint (not peer reviewed)*. https://doi.org/10.64898/2026.07.01.735889

### Dopamine, prediction error and the tilt mechanism (added research basis)

- Schultz, W., Dayan, P., & Montague, P. R. (1997). A neural substrate of prediction and reward. *Science, 275*, 1593–1599. https://doi.org/10.1126/science.275.5306.1593
- Frank, M. J., Seeberger, L. C., & O'Reilly, R. C. (2004). By carrot or by stick: Cognitive reinforcement learning in parkinsonism. *Science, 306*, 1940–1943. https://doi.org/10.1126/science.1102941
- Shen, W., Flajolet, M., Greengard, P., & Surmeier, D. J. (2008). Dichotomous dopaminergic control of striatal synaptic plasticity. *Science, 321*, 848–851. https://doi.org/10.1126/science.1160575
- Frank, M. J., Doll, B. B., Oas-Terpstra, J., & Moreno, F. (2009). Prefrontal and striatal dopaminergic genes predict individual differences in exploration and exploitation. *Nature Neuroscience, 12*, 1062–1068. https://doi.org/10.1038/nn.2342
- Kravitz, A. V., Tye, L. D., & Kreitzer, A. C. (2012). Distinct roles for direct and indirect pathway striatal neurons in reinforcement. *Nature Neuroscience, 15*, 816–818. https://doi.org/10.1038/nn.3100
- Cox, S. M. L., Frank, M. J., Larcher, K., et al. (2015). Striatal D1 and D2 signaling differentially predict learning from positive and negative outcomes. *NeuroImage, 109*, 95–101. https://doi.org/10.1016/j.neuroimage.2014.12.070
- Lee, S. J., et al. (2021). Cell-type-specific asynchronous modulation of PKA by dopamine in learning. *Nature, 590*, 451–456. https://doi.org/10.1038/s41586-020-03050-5
- Zachry, J. E., et al. (2024). D1 and D2 medium spiny neurons in the nucleus accumbens core have distinct and valence-independent roles in learning. *Neuron, 112*, 835–849.e7. https://doi.org/10.1016/j.neuron.2023.11.023
- Lowet, A. S., et al. (2025). An opponent striatal circuit for distributional reinforcement learning. *Nature, 639*, 717–726. https://doi.org/10.1038/s41586-024-08488-5
- Romero Pinto, S., & Uchida, N. (2025). Tonic dopamine and biases in value learning linked through a biologically inspired reinforcement learning model. *Nature Communications, 16*, 7529. https://doi.org/10.1038/s41467-025-62280-1
- Kahnt, T., & Schoenbaum, G. (2025). The curious case of dopaminergic prediction errors and learning associative information beyond value. *Nature Reviews Neuroscience, 26*, 169–178. https://doi.org/10.1038/s41583-024-00898-8

### Primary and contextual sources retained from the three original sections

- Moretti, P., & Muñoz, M. A. (2013). *Griffiths phases and the stretching of criticality in brain networks*. Nature Communications, 4, 2521. https://doi.org/10.1038/ncomms3521
- Ódor and colleagues (2015). Hierarchical network dynamics and Griffiths phases. *Scientific Reports*. https://www.nature.com/articles/srep14451
- Beggs, J. M., & Plenz, D. (2003). *Neuronal avalanches in neocortical circuits*. Journal of Neuroscience, 23, 11167–11177. https://doi.org/10.1523/JNEUROSCI.23-35-11167.2003
- Botvinick, M. M., & Weinstein, A. (2014). Hierarchical reinforcement learning and temporally extended skills (source referenced in prior draft). https://pubmed.ncbi.nlm.nih.gov/25267822/
- Dezfouli, A., & Balleine, B. W. (2013). Learned action sequences and goal-directed control (source referenced in prior draft). https://pubmed.ncbi.nlm.nih.gov/24339762/
- Stachenfeld, K. L., Botvinick, M. M., & Gershman, S. J. (2017). *The hippocampus as a predictive map*. Nature Neuroscience, 20, 1643–1653. https://doi.org/10.1038/nn.4650
- Gershman, S. J. (2018). *The successor representation: Its computational logic and neural substrates*. Journal of Neuroscience, 38, 7193–7200. https://doi.org/10.1523/JNEUROSCI.0151-18.2018
- Li, Li, & Wang (2025). Cortical timescale hierarchies and near-critical network modelling in marmosets (source referenced in prior draft). https://www.nature.com/articles/s41467-025-66699-4
- Human intracranial EEG study (2025), cited in prior temporal-dynamics draft. https://pmc.ncbi.nlm.nih.gov/articles/PMC11984084/
- Zeraati and colleagues (2026). Review of neural timescale mechanisms (source referenced in prior draft). https://www.nature.com/articles/s41593-026-02343-8

The source blocks above include both newly integrated and inherited references. Their inclusion is **not** a claim that the complete Trident-G synthesis has been independently validated. The 2026 Xue study is explicitly a non-peer-reviewed preprint; other sources range from computational proposals to invasive recordings and human imaging. Bibliographic details of older inherited sources should be checked before publication. Bibliographic details should be verified and standardised before publication.

---

## Theoretical conclusion

Trident-G Version 0.3 is a proposal about **regulated coordination and recursive change**. Its most distinctive claim is that general intelligence may depend on a system's ability to preserve efficient specialised operations while selectively reorganising their relationships under novel demands. A viable homeostatic corridor constrains this process; hierarchical modularity makes parallel specialised and integrative cognition possible; extended Griffiths-phase-like dynamics may, under appropriate conditions, broaden the system's effective response repertoire across timescales. Gf synthesis generates and tests relational structures, and dual-pathway Gc consolidation can convert validated structures into both efficient skills and richer schemas. Through asymmetrical capacity interactions and reciprocal niche construction, these changes can modify the conditions of subsequent learning.

**The next decisive step is not another conceptual layer.** It is a small computational model in which the hierarchical controller, cusp controller and Griffiths-phase network can be independently ablated, followed by preregistered behavioural tests of novel skill composition, temporal-horizon coordination and delayed invariant transfer.
