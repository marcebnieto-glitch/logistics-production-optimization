# Production Planning Optimization — Falcon Die Casting Company

Linear programming project for production scheduling optimization across a 12-week horizon.

> **Individual project** — developed independently as part of the Master in Data Analytics for Business, UPF Barcelona School of Management.

## Objective
Model and solve a production planning problem for a die casting company, minimizing overtime hours while satisfying weekly demand under real operational constraints.

## Problem
Falcon Die Casting Company must plan production across 5 machines and multiple part types over 12 weeks. The challenge: satisfy variable demand while respecting machine capacities, yield rates, setup times, and overtime limits.

## Three models compared

**Model I — Independent weekly planning (no inventory)**
- Each week optimized separately
- No stock carryover allowed
- Result: infeasible in week 11 (demand exceeds maximum capacity)

**Model II — Cross-week planning with inventory**
- Production can be anticipated in low-demand weeks
- Inventory acts as a buffer for demand peaks
- Result: feasible across all 12 weeks, more stable overtime distribution

**Model III — Yield improvement scenario**
- Simulates improved machine yield (% valid parts)
- Higher effective output per hour without adding physical resources
- Result: lower total hours needed to meet the same demand

## Key findings
- Allowing inventory (Model II) eliminates infeasibility and reduces operational risk
- Higher overtime in Model II vs Model I reflects a realistic, complete plan — not inefficiency
- Yield improvements (Model III) increase system capacity without additional investment

## Tools & Libraries
- Python, PuLP (linear programming)
- Pandas, NumPy
- Matplotlib, Seaborn

## Concepts applied
- Linear programming (LP) formulation
- Decision variables, objective function, constraints
- Inventory modeling
- Machine capacity and setup time constraints
- Sensitivity analysis across scenarios

## Individual project
Developed independently as part of the Master in Data Analytics for Business — UPF Barcelona School of Management.
