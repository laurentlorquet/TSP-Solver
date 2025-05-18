## 🧪 Test Scenarios

This project includes experimental tests with different ACO parameter settings to evaluate their effect on solution quality and runtime.

### ✅ Test 1: High Colony Size (Brute-Force-Like)
- **Goal:** Examine how a large number of ants affects convergence speed.
- **Setup:**
  - Cities: 25 randomly placed
  - Ants: 50
  - Iterations: 200
- **Observations:**
  - Faster convergence to high-quality solutions
  - Higher runtime per iteration
  - Behaves similarly to brute-force but guided by pheromones

---

### ✅ Test 2: High Iteration Count (Slow and Steady)
- **Goal:** Determine the impact of excessive iterations on convergence.
- **Setup:**
  - Cities: 25 randomly placed
  - Ants: 25
  - Iterations: 500
- **Observations:**
  - Solution quality improves over time, but gains plateau
  - Many iterations go unused after convergence
  - Increased total runtime with marginal benefit after early epochs
- **Insight:** Choosing an optimal iteration threshold is critical to avoid unnecessary computation.
