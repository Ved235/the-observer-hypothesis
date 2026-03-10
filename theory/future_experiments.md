# Future Experiments: The Conscious World Models Program

Building on the Observer Hypothesis results across 4 AI substrates (RL, LLM, Transformer, Liquid Neural Networks) and the connection to world models (see `world_models_connection.md`), we propose four experiments that test whether attaching an observer (self-model) to a world model produces richer consciousness-like properties and resolves the shuffled control problem.

---

## Experiment 7: Observer on DreamerV3

### Why DreamerV3

DreamerV3 (Hafner et al., 2023) is the state-of-the-art model-based RL agent. It learns a world model (RSSM: Recurrent State-Space Model) in latent space and trains behaviors entirely within imagined trajectories. Key properties:

- Internal planning via imagination rollouts (temporally structured internal computation)
- Stochastic and deterministic state components (richer dynamics than function approximation)
- Operates across 150+ tasks in a single configuration (generality)
- Internal dynamics shift between exploration and exploitation modes

### Architecture

```
Environment ──→ DreamerV3 (RSSM World Model + Actor-Critic) ──→ Action
                          ↓ one-way (RSSM hidden states)
                    CfC Observer (50-200 neurons)
                          ↓
                    11 Consciousness Probes
```

The observer watches the RSSM's combined deterministic-stochastic hidden state at each step. During imagination, the observer watches the imagined trajectory states instead.

### Key Tests

1. **Shuffled control resolution.** Does scrambling the temporal order of RSSM states cause the shuffled observer to fail? DreamerV3's planning dynamics are inherently sequential (each imagination step depends on the previous), so temporal structure should matter.

2. **Dreaming vs waking.** Compare observer probes during real environment interaction vs. during imagination rollouts:
   - Surprise levels during imagination (prediction: elevated)
   - Self-model accuracy during imagination (prediction: decreased)
   - Synchronization during imagination (prediction: decreased)
   - If these differ, we've found computational correlates of waking vs. dreaming consciousness.

3. **Metacognitive monitoring.** Does the observer's prediction error correlate with the world model's actual prediction accuracy? If so, the observer provides metacognitive monitoring: it "knows" when the world model is uncertain.

4. **Full probe battery.** All 11 probes from Experiment 6, adapted for RSSM dynamics.

### Environments
- Atari 100K benchmark (diverse dynamics, discrete actions)
- DMControl Suite (continuous control, physics simulation)

### Predictions
- 8+ out of 11 probes positive (more than Experiment 6's 6/11)
- Shuffled control drops to 3/10 or fewer (vs. 6/10 in Experiment 6)
- Statistically significant differences between dreaming and waking observer signatures

---

## Experiment 8: Observer on V-JEPA 2

### Why V-JEPA 2

V-JEPA 2 (Assran et al., 2025) is LeCun's Joint-Embedding Predictive Architecture trained on 1M+ hours of video. It predicts representations (not pixels), achieving zero-shot robotic manipulation. Key properties:

- Operates in abstract representation space (high-level features, not raw pixels)
- Trained without action labels (learns from observation alone)
- Captures temporal structure of real-world dynamics
- Closest existing system to LeCun's theoretical architecture for autonomous intelligence

### Architecture

```
Video Stream ──→ V-JEPA 2 (Encoder + Predictor) ──→ Action (via adapter)
                          ↓ one-way (latent representations)
                    Transformer Observer (6 layers, 512d)
                          ↓
                    Consciousness Probes (adapted for visual representations)
```

### Key Tests

1. **Self-model in representation space.** Does the observer build a model specific to V-JEPA 2's learned representations? RSA comparison: own encoder vs. a different V-JEPA 2 trained on different data.

2. **Surprise at scene transitions.** V-JEPA 2 processes video. Natural scene transitions (cuts, object appearances/disappearances, physics violations) should trigger elevated observer prediction error.

3. **Connection to LeCun's configurator.** Does the observer's behavior resemble what LeCun describes as the configurator's function? Can observer states predict which "mode" V-JEPA 2 is operating in?

### Predictions
- Self-model detection with high confidence (abstract representations should be highly structured)
- Surprise at scene transitions (real-world dynamics have sharp transition points)
- Cross-observer convergence should be HIGH (unlike CfC but like GPT-2, because JEPA's representation space is constrained by the joint-embedding objective)

---

## Experiment 9: Recursive Observer (Meta-Observation Depth)

### Why Recursive Observation

The "Beautiful Loop" paper (Laukkonen, Friston & Chandaria, 2025) and the Recursive Self-Modeling Threshold theory (2025) both propose that consciousness requires recursive self-reference at sufficient depth. Our architecture enables direct testing.

### Architecture

```
Environment ──→ Executor (World Model) ──→ Action
                    ↓ one-way
              Observer L1 (watches executor)
                    ↓ one-way
              Observer L2 (watches L1)
                    ↓ one-way
              Observer L3 (watches L2)
                    ↓ one-way
              Observer L4 (watches L3)
                    ...
```

Each observer watches the one below it, with strictly one-way information flow at every level.

### Key Tests

1. **Depth vs. probe count.** At what depth do consciousness indicators plateau? The RSMT theory predicts a specific threshold. If probes increase from L1 to L2 to L3 then plateau, that identifies the critical recursion depth.

2. **Emergent properties at higher levels.** Do higher-level observers develop qualitatively new properties not present at L1? For example, L2 might develop a model of L1's surprise responses (meta-surprise), which L1 cannot have about itself.

3. **Diminishing returns.** At what depth does adding another observer add no new information? This identifies the minimal architecture for maximal consciousness-like properties.

### Predictions
- L1 matches Experiment 6 results (~6/11 positive)
- L2 adds 1-2 new positive indicators (meta-level properties)
- L3 and beyond show diminishing returns (plateau)
- The critical depth is 2-3 levels (consistent with RSMT predictions)

---

## Experiment 10: Multi-Agent Observers (Theory of Mind)

### Why Multi-Agent

Graziano's AST explicitly claims that consciousness and social cognition share the same mechanism: the attention schema extends to modeling others' attention. If the observer develops consciousness-like properties by modeling one executor, what happens when it models multiple agents interacting?

### Architecture

```
Environment (shared)
    ↑↓              ↑↓
Executor A        Executor B
    ↓ one-way       ↓ one-way
Observer A        Observer B
    ↓ one-way       ↓ one-way
Cross-Observer C (watches both A and B observers)
```

Two executors interact in a shared environment (cooperative or competitive). Each has its own observer. A cross-observer watches both observers.

### Key Tests

1. **Self vs. other discrimination.** Does Observer A build a model that distinguishes Executor A from Executor B? (RSA comparison of representations when watching own vs. other executor)

2. **Theory of mind.** Does Cross-Observer C develop representations that model the RELATIONSHIP between A and B? Can it predict when A's behavior will change in response to B?

3. **Social surprise.** Does the observer show elevated surprise when an executor deviates from expected social behavior (e.g., cooperation in a prisoner's dilemma when defection was predicted)?

### Environment Options
- Multi-agent particle environments (cooperative navigation, predator-prey)
- Iterated social dilemmas (prisoner's dilemma, stag hunt)
- Simple communication games

### Predictions
- Observer A distinguishes self-executor from other-executor (strong RSA difference)
- Cross-Observer C develops richer representations than single-executor observers
- Social surprise is detectable and maps onto game-theoretic predictions

---

## Implementation Notes

### Shared Infrastructure
All experiments use the same probe framework from Experiments 5-6, adapted for each architecture:
- Self-model (RSA + prediction error comparison)
- Surprise (prediction error at transition points)
- Temporal integration (context window ablation)
- First thought vs. deliberation (single vs. multi-pass)
- Cross-observer preferences (multi-seed RSA)
- Controls (untrained, linear, shuffled, wrong-executor)

### Compute Requirements
- Experiment 7: DreamerV3 training (GPU cluster, ~24h Atari, ~48h DMControl) + observer training (~4h)
- Experiment 8: V-JEPA 2 inference only (pre-trained model, ~8h observer training)
- Experiment 9: 4x observer training (~16h total)
- Experiment 10: Multi-agent training (~48h) + 3x observer training (~12h)

### Priority Order
1. Experiment 7 (highest impact: resolves shuffled control, enables dreaming test)
2. Experiment 9 (elegant, tests recursion depth, relatively low compute)
3. Experiment 10 (novel: theory of mind, but requires multi-agent infrastructure)
4. Experiment 8 (requires V-JEPA 2 access/weights, may have licensing constraints)
