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

The explore–exploit tilt can be written:

$$
\delta_t=u_t+\sum_n\lambda_{n,t}\psi_n(\mathbf z_{n,t},K_{n,t})
+\boldsymbol\omega^\top\mathbf b_t.
$$

Here $u_t$ represents strategic control, $\lambda_{n,t}$ effective coupling to niche $n$, $\psi_n$ the niche's current pressure on policy selection, and $\mathbf b_t$ the active Gf branches. More coupling is not always better: inaccurate, captured or hostile coupling can also distort control.

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

## 3.1 Selective recruitment and joint action

A module's recruitment depends on task cues, the current plan, context and evidence of mismatch:

$$
\gamma_{j,t}=\operatorname{Gate}_j
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

# 8. Gf→Gc→Gf banking builds both knowledge and modules

Consolidation has at least two related outputs.

**Fast Gc compilation** produces readily available procedures, local control policies, task rules and skilled subroutines. Some may become relatively autonomous and recruitable as modules.

**Slow Gc integration** produces gist, general relational schemas and representational organisation accumulated across episodes. This can reshape which variables, constraints and connections are salient during later Gf search.

These are functional pathways and different characteristic learning timescales, not assertions that each can be assigned to a single isolated anatomical site.

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

The earliest computational implementation should **freeze slow developmental variables** and specify concrete forms for $\mathcal S$, $\mathcal M$, $\mathcal A$, $\operatorname{Gate}$, $f_j$ and $\mathcal B$. Meta-efficacy $\eta$, coherence $\chi$, homeostatic conditions $\mathbf h$, and $F^\star$ presently enter as inputs or slow latent quantities: their own update laws are open questions. Version 0.3 is therefore a *structured candidate theory*, not yet a closed, identifiable model.

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

**A3. Anticipated load and exploration–exploitation tilt**

$$
\begin{aligned}
G&=\mathscr G(\mathbf c,\eta,\chi,\mathbf h,K^{Gc},\mathbf b,\mathbf z,\text{goal}),\\
\delta&=u+\sum_n\lambda_n\psi_n(\mathbf z_n,K_n)+\boldsymbol\omega^\top\mathbf b.
\end{aligned}
$$

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

**A7. Skill gating and assembled action**

$$
\gamma_j=\operatorname{Gate}_j(\mathbf o_{t^-},\mathbf r^\star_{t^-},e_{j,t^-},\mathbf z,\eta),\qquad
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

The references above are inherited from the three source sections; their inclusion is **not** a claim that the complete Trident-G synthesis has been independently validated. Bibliographic details should be verified and standardised before publication.

---

## Theoretical conclusion

Trident-G Version 0.3 is a proposal about **regulated coordination and recursive change**. Its most distinctive claim is that general intelligence may depend on a system's ability to preserve efficient specialised operations while selectively reorganising their relationships under novel demands. A viable homeostatic corridor constrains this process; hierarchical modularity makes parallel specialised and integrative cognition possible; extended Griffiths-phase-like dynamics may, under appropriate conditions, broaden the system's effective response repertoire across timescales. Gf synthesis generates and tests relational structures, and dual-pathway Gc consolidation can convert validated structures into both efficient skills and richer schemas. Through asymmetrical capacity interactions and reciprocal niche construction, these changes can modify the conditions of subsequent learning.

**The next decisive step is not another conceptual layer.** It is a small computational model in which the hierarchical controller, cusp controller and Griffiths-phase network can be independently ablated, followed by preregistered behavioural tests of novel skill composition, temporal-horizon coordination and delayed invariant transfer.
