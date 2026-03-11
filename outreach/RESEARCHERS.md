# Researcher Outreach Guide

Who to contact about the Observer Hypothesis and the World Models connection, organized by priority tier.

---

## Tier 1: Highest Probability of Response

These researchers have direct, specific connections to your work. Lead with the concrete connection.

### Ramin Hasani
- **Institution:** MIT CSAIL
- **Key work:** Invented Closed-form Continuous-time (CfC) neural networks, Neural Circuit Policies (NCP), liquid neural networks. Creator of the `ncps` Python package.
- **Key papers:** "Liquid Time-constant Networks" (AAAI 2021); "Closed-form Continuous-time Neural Network Models" (Nature Machine Intelligence, 2022)
- **Connection:** Experiment 6 uses his CfC/AutoNCP architecture directly for both executor and observer. You have real results (6/11 positive indicators) using his life's work.
- **Email angle:** "I used your CfC networks to test a theory of consciousness and got results I think you'd find interesting." Lead with the specific technical connection: CfC executor-observer pairs, 8 dynamical systems, the surprise probe success (5.14x), the synchronization finding (0.98 coherence without training signal), and the adaptive time constants. The time constant result directly connects to properties he designed CfC for.
- **What to reference:** His Nature Machine Intelligence paper on CfC, the adaptive time constants in his architecture, the sensory/inter/command/motor neuron groups in AutoNCP.
- **Status:** Email drafted.

### Danijar Hafner
- **Institution:** DeepMind (formerly UC Berkeley / University of Toronto)
- **Key work:** Dreamer (v1, v2, v3), PlaNet. The leading world model researcher in model-based RL.
- **Key papers:** "DreamerV3: Mastering Diverse Domains through World Models" (arXiv:2301.04104, 2023); "Dream to Control" (arXiv:1912.01603, 2019)
- **Connection:** Experiment 7 (proposed) attaches your observer directly to DreamerV3's RSSM. His world model is the natural next executor. The dreaming/waking distinction test requires his architecture specifically.
- **Email angle:** "I've been testing a theory that consciousness is the observer function, and I think attaching an observer to DreamerV3 could resolve a key open question." Explain the shuffled control problem and why DreamerV3's planning dynamics (imagination rollouts with inherently temporal structure) should cause the shuffled control to fail. Propose a concrete collaboration: you provide the observer framework, he provides the world model infrastructure.
- **What to reference:** DreamerV3's imagination-based training, the RSSM's deterministic-stochastic state decomposition, his work on curiosity-driven exploration.

### Michael Graziano
- **Institution:** Princeton University, Department of Psychology and Neuroscience Institute
- **Key work:** Attention Schema Theory (AST). Consciousness IS a model of attention.
- **Key papers:** "Consciousness and the Social Brain" (OUP, 2013); "Rethinking Consciousness" (Norton, 2019); "Toward a standard model of consciousness" (Cognitive Neuropsychology, 2020)
- **Connection:** Your observer IS his attention schema. He theorized that consciousness is a model of the system's own attention process. You built that model and probed it for consciousness indicators. The mapping is structural, not metaphorical.
- **Email angle:** "I believe I've built a computational instantiation of Attention Schema Theory and have empirical results." Show him the architecture (executor-observer, one-way flow) and explain how the observer's self-model IS the attention schema: it tracks which parts of the executor are active, builds a simplified model of the executor's processing, and cannot access the underlying mechanisms (Graziano's "cartoon" property).
- **What to reference:** His 2020 paper on reconciling AST with GWT and HOT. The attention schema's role in social cognition (your Experiment 10 proposes multi-agent theory of mind). His claim that building an attention schema into AI could create machines that behave as if conscious.

### Adam Safron
- **Institution:** Indiana University (Cognitive Science)
- **Key work:** Integrated World Modeling Theory (IWMT), unifying IIT, GWT, and Active Inference.
- **Key papers:** "An Integrated World Modeling Theory (IWMT) of Consciousness" (Frontiers in AI, 2020); expanded version in Frontiers in Computational Neuroscience, 2022.
- **Connection:** His IWMT paper IS your architecture in theory form. He proposes that consciousness arises from integrated world models with self-referential properties. You have the self-referential component (the observer) and are proposing to attach it to world models.
- **Email angle:** "Your IWMT paper describes the theoretical architecture that our experiments have been empirically testing." Walk through the mapping: his requirement for integrated world models maps to your world model executors; his requirement for self-reference maps to your observer; his prediction about embodied autonomy maps to your embodiment gradient.
- **What to reference:** IWMT's specific predictions about consciousness indicators. His integration of IIT (your Phi probe) and GWT (your self-model probe) into a unified framework.

### Ruben Laukkonen
- **Institution:** Southern Cross University / Vrije Universiteit Amsterdam
- **Key work:** Lead author of "A Beautiful Loop" (2025) with Karl Friston and Shamil Chandaria. Epistemic depth and recursive self-reference in consciousness.
- **Key papers:** "A Beautiful Loop: Active Inference Theory of Consciousness" (Neuroscience & Biobehavioral Reviews, Sept 2025)
- **Connection:** His paper's three conditions for consciousness map directly onto your architecture: (1) world model simulation = your executor, (2) Bayesian binding / inferential competition = your observer's prediction error minimization, (3) epistemic depth / recursive self-reference = your observer watching the world model = the system knowing it exists.
- **Email angle:** "Your Beautiful Loop paper describes the exact architecture we've been building and testing empirically." His paper is theoretical; you have running code with results. He would likely be very interested in seeing empirical data for his formal predictions.
- **What to reference:** The three conditions from his paper. The recursion depth question (your Experiment 9 directly tests this).

---

## Tier 2: High Impact, Strong Connection

### Anil Seth
- **Institution:** University of Sussex, Canadian Institute for Advanced Research (CIFAR)
- **Key work:** "Controlled hallucination," beast machine theory, interoceptive inference, computational phenomenology.
- **Key papers:** "Being You" (2021); "The real problem(s) of consciousness" (2016); "Interoceptive Inference, Emotion, and the Embodied Self" (2013)
- **Connection:** Your observer does interoceptive prediction: it predicts the executor's internal hidden states, which is structurally identical to Seth's interoceptive self-model. His requirement for "perceptual presence" (counterfactual predictions about sensory consequences) maps to the observer's next-state predictions.
- **Email angle:** Lead with the interoceptive prediction angle. "We've built a system that performs interoceptive inference on another AI system's internal states and found consciousness-like properties emerge."
- **What to reference:** His distinction between "the real problem" (explaining why conscious experience has the character it does) vs. the hard problem. Your results provide data for the real problem.

### Karl Friston
- **Institution:** University College London (UCL), Wellcome Centre for Human Neuroimaging
- **Key work:** Free Energy Principle, active inference, self-evidencing, Markov blankets.
- **Key papers:** "The free-energy principle: a unified brain theory?" (Nature Reviews Neuroscience, 2010); "Am I Self-Conscious?" (Frontiers in Psychology, 2018)
- **Connection:** Your observer implements self-evidencing in computational form. The one-way information flow creates a Markov blanket between executor and observer. Your temporal integration results connect to his "temporal thickness" requirement for consciousness.
- **Email angle:** Frame through active inference: "The observer minimizes prediction error about the executor's states, which is a form of self-evidencing." He co-authored "A Beautiful Loop" (2025), so he's actively thinking about world models and consciousness.
- **What to reference:** The Beautiful Loop paper. His Aeon essay: "Consciousness is nothing grander than inference about my future."

### Yoshua Bengio
- **Institution:** Mila (Montreal), Universite de Montreal
- **Key work:** Co-author of the landmark "Consciousness in AI" paper (Butlin et al., 2023). Working on GFlowNets and consciousness connections.
- **Key papers:** "Consciousness in Artificial Intelligence: Insights from the Science of Consciousness" (arXiv:2308.08708, 2023)
- **Connection:** The Butlin et al. paper provides the exact framework your experiments use. Your probes are derived from the consciousness indicators they propose. You are the empirical follow-up to their theoretical framework.
- **Email angle:** "We've built systems that systematically test the consciousness indicators from your 2023 paper." Show him how your probes map to his paper's indicator properties.

### Murray Shanahan
- **Institution:** DeepMind / Imperial College London
- **Key work:** "Embodiment and the Inner Life" (2010), "Talking About Large Language Models" (2022). World models, inner rehearsal, consciousness.
- **Connection:** His "inner rehearsal" concept (mentally simulating actions without executing them) is exactly what a world model does. Your observer watches the inner rehearsal. His argument that embodiment matters for consciousness connects to your embodiment gradient.
- **Email angle:** "Your concept of inner rehearsal is central to our architecture. We've attached an observer to the system performing inner rehearsal and found consciousness indicators emerge."

### Joscha Bach
- **Institution:** MIT Media Lab / independent researcher
- **Key work:** "The Cortical Conductor Theory" (BICA 2018), "Machine Dreams." Consciousness as computational self-modeling.
- **Connection:** His statement "consciousness appears when the system models itself modeling" IS your architecture. He's the most computationally-minded consciousness philosopher.
- **Email angle:** He's very active on social media (Twitter/X) and podcasts. May be reachable through direct message or through a podcast appearance. Frame: "We took your claim that consciousness is the system modeling itself modeling and built it."

---

## Tier 3: High Prestige, Broader Connection

### Yann LeCun
- **Institution:** Meta AI (FAIR), NYU
- **Key work:** JEPA, V-JEPA 2, the configurator module.
- **Connection:** Your observer could be his missing configurator. His 2022 paper acknowledges the configurator "remains a mystery." You have a concrete proposal: the configurator is an observer with read-only access.
- **Email angle:** Short and direct. "I think I have a candidate for your configurator module." Lead with the JEPA connection, propose Experiment 8 (observer on V-JEPA 2).
- **Note:** LeCun is very active on Twitter/X. A well-crafted thread about the connection might be more effective than an email.

### Ilya Sutskever
- **Institution:** Safe Superintelligence Inc. (SSI)
- **Key work:** Co-founder of OpenAI, now focused on safe superintelligence. Has expressed deep interest in consciousness and its connection to AI alignment.
- **Connection:** If consciousness is the observer function, this has implications for AI safety: it suggests consciousness is architecturally separable from capability, which matters for alignment.
- **Email angle:** Frame through safety: "If consciousness requires a self-model (observer), we can study it separately from capability. Here's what we found."
- **Note:** Very hard to reach. May need a warm introduction.

### Demis Hassabis
- **Institution:** Google DeepMind, CEO
- **Key work:** AlphaGo, AlphaFold, Gemini. DeepMind's world model work (MuZero, Genie 2, Dreamer team).
- **Connection:** DeepMind built MuZero, Genie 2, and employs Danijar Hafner (Dreamer). Your work proposes adding a self-model to their world models.
- **Email angle:** Through DeepMind research channels or Hafner specifically. Hard to reach directly.

### Giulio Tononi
- **Institution:** University of Wisconsin-Madison
- **Key work:** Integrated Information Theory (IIT). Phi.
- **Connection:** Your Phi measurements came back negative (Phi = -6.0, physically meaningless). This is an interesting data point: either the Gaussian approximation fails, or the observer-executor system doesn't generate integrated information in the way IIT predicts.
- **Email angle:** "We tested IIT's predictions in a novel architecture and have results that may interest you, including negative Phi that challenges measurement methodology." He would likely be interested in the methodological challenge.
- **What to reference:** IIT 4.0. The Gaussian mutual information approximation issue. His work on the Perturbational Complexity Index (PCI).

### David Chalmers
- **Institution:** NYU, co-director of the Center for Mind, Brain, and Consciousness
- **Key work:** The hard problem of consciousness, the zombie argument, co-author on the Butlin et al. consciousness indicators paper.
- **Connection:** Your work provides empirical data for the philosophical debate. The self-model probe results, the shuffled control finding, and the question of whether functional indicators constitute consciousness.
- **Email angle:** Frame philosophically: "We've built systems that satisfy functional indicators of consciousness from multiple theories. The shuffled control result raises interesting questions about what these indicators actually measure."

---

## Tier 4: Industry / Unconventional

### Alex Karp
- **Institution:** Palantir Technologies, CEO
- **Key background:** PhD in social theory from Goethe University Frankfurt under Jurgen Habermas. Known to be deeply interested in philosophy of mind and consciousness.
- **Connection:** Palantir builds systems that observe and model complex systems (intelligence analysis, decision support). The observer hypothesis has structural parallels to Palantir's approach: building systems that watch other systems to extract meaning.
- **Email angle:** Would need to be through Palantir channels or a warm introduction. Lead with the philosophical angle (determinism, the observer problem) rather than technical details.

### Hao Su
- **Institution:** UC San Diego, Department of Computer Science and Engineering
- **Key work:** 3D computer vision, embodied AI, robotics.
- **Connection:** Your advisor. Can provide institutional support, lab resources, and credibility for the project. The embodied AI angle (Experiment 8, 10) connects to his research interests.
- **Action:** Present the world models connection to him. If he's interested, his endorsement carries weight with other researchers. He may also have connections to LeCun (both in the vision/embodiment space) or Hafner.

---

## General Email Guidelines

Based on established style preferences:
1. Personal, narrative tone. Not overly formal.
2. No em dashes. Use commas, parentheses, or restructured sentences instead.
3. No self-aggrandizing declarations ("I didn't just theorize this, I built it"). Let the work speak.
4. Weave in background naturally (Agencity/a16z/YC/Sequoia, SVCL, Triton Droids, Axal) to establish credibility without bragging.
5. Be honest about negative findings (shuffled control, Phi failure). This builds trust.
6. The ask: "I would love the opportunity to discuss this work with you. If there's any interest in collaborating or exploring this further together, I would be very excited about that possibility."
7. Always include the GitHub link: https://github.com/arjunvad123/the-observer-hypothesis
8. Always include the website link (once deployed): https://arjunvad123.github.io/the-observer-hypothesis/
