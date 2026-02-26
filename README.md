# Quantum-Inspired PPO for Optimized Network Routing

A reinforcement learning system that **improves routing decisions in dynamic networks** by augmenting Proximal Policy Optimization (PPO) with quantum-inspired representations (superposition/interference-style effects via complex-valued layers). The project includes a realistic packet-level simulator, strong baselines, and an evaluation pipeline focused on delivery ratio, latency, throughput, and convergence speed.

## Why this matters
Modern networks face shifting traffic, congestion, and failures—static routing and simple heuristics often struggle under non-stationarity. This repo explores how quantum-inspired neural components can improve exploration and policy learning stability for adaptive routing.

## Highlights
- **Quantum-inspired policy network:** Complex-valued layers + “measurement” style readout for richer state representations and exploration.
- **Enhanced PPO agent:** PPO extended with quantum-inspired encoder/layers while keeping the PPO training loop familiar and reproducible.
- **Realistic network simulation:** Random, scale-free, and small-world topologies with dynamic traffic, congestion, and failures.
- **Multi-objective evaluation:** Packet delivery, end-to-end delay, throughput, and utilization.
- **Strong baselines included:** OSPF, ECMP, Q-Routing, DQN, PPO for fair comparison.

## Results (from this repo’s experiments)
Quantum-inspired PPO vs. classical baselines:
- **+4.3%** packet delivery ratio (PDR)
- **-12.7%** end-to-end delay
- **+6.2%** throughput
- **30–33%** faster convergence

## References
- Schulman, J., Wolski, F., Dhariwal, P., Radford, A., & Klimov, O. (2017). *Proximal Policy Optimization Algorithms*. arXiv:1707.06347. https://arxiv.org/abs/1707.06347
- Nielsen, M. A., & Chuang, I. L. (2010). *Quantum Computation and Quantum Information* (10th Anniversary ed.). Cambridge University Press.
- Biamonte, J., Wittek, P., Pancotti, N., Rebentrost, P., Wiebe, N., & Lloyd, S. (2017). *Quantum machine learning*. Nature, 549, 195–202. https://doi.org/10.1038/nature23474
