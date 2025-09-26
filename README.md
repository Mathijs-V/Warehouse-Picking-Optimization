# Warehouse-Picking-Optimization

# Portfolio Minor High Tech AI-Systems

## Part 1 – The Learning Plan

### 1a. Personal Learning Plan

#### Student Profile
I am Mathijs Vandooren, a software engineering student at Fontys with a strong background in backend development, data handling, and e-commerce systems. I work at an e-commerce company (Pyjamaonline) with an average of ~500 orders/day in the winter, where I directly experience the challenges of warehouse efficiency.  
My specific interest lies in applying Artificial Intelligence to real-world logistics problems. After completing this minor, I aim to contribute to the optimization of warehouse operations by integrating AI-driven decision-making into practical systems.

#### Self-reflection
So far, my strengths are in:
- Backend development (Node.js, Django, APIs)
- Data integration (e-commerce platforms, logistics APIs)
- Practical understanding of warehouse operations

Areas I want to improve:
- Applying reinforcement learning (RL) to real-world problems
- Designing AI experiments with measurable KPIs
- Simulation and evaluation of AI models in logistics settings

#### Personal Learning Objectives
- Gain hands-on experience with reinforcement learning applied to optimization problems.
- Learn to design, train, and evaluate AI models against classical algorithms.
- Improve in structuring large projects with a research-oriented mindset.
- Strengthen reflection and documentation skills by maintaining a weekly portfolio.

---

### 1b. Theoretical Learning Plan

#### Context
Order picking is one of the most labor-intensive processes in warehouses, representing up to 50% of operational costs. For e-commerce companies with 500+ orders/day, multi-item orders often result in inefficient walking distances and increased cycle times.  
Traditionally, heuristic methods (e.g., shortest path, TSP solvers) are used. However, recent research suggests reinforcement learning (RL) can adaptively optimize routes under dynamic conditions. This project explores whether RL can outperform classical heuristics in a medium-scale warehouse.

#### Main Research Question
*Can reinforcement learning optimize warehouse pick-paths more effectively than heuristic algorithms, in terms of walking distance and cycle time, for a mid-sized e-commerce warehouse?*

#### Theoretical Learning Objectives
- Understand existing heuristic approaches to warehouse routing (TSP, nearest neighbor).
- Learn the fundamentals of reinforcement learning for path optimization.
- Apply RL to a simulated warehouse environment and compare performance to heuristics.
- Evaluate AI models based on KPIs: meters walked, cycle time, picks/hour.

#### Learning Strategy
1. Literature research on warehouse routing & RL (Weeks 1–3).  
2. Data preparation: map warehouse layout & extract order data (Weeks 1–3).  
3. Baseline implementation: OR-Tools heuristics for TSP (Weeks 4–6).  
4. Simulation: build digital twin of warehouse in SimPy (Weeks 4–8).  
5. AI approach: implement RL agent for path optimization (Weeks 9–15).  
6. Experimentation: run comparative studies on KPIs (Weeks 16–20).  
7. Reporting & reflection: document results, portfolio updates, prepare demo (Weeks 21–24).  

#### Goals & Deliverables
- **Simulation environment** of the warehouse.  
- **Baseline results** with heuristic routing.  
- **RL agent** trained to optimize pick paths.  
- **Comparative study** with KPIs.  
- **Final report & presentation** with conclusions and reflections.

---

### Timeline (24 Weeks)

| Week(s) | Focus | Deliverables |
|---------|-------|--------------|
| 1–2 | Literature study, define KPIs, portfolio setup | Summary of related work, initial context write-up |
| 3 | Warehouse data preparation (layout, orders) | Digital layout representation & dataset |
| 4–6 | Baseline routing (heuristics: OR-Tools, nearest neighbor) | Scripts + baseline performance metrics |
| 7–8 | Simulation environment (SimPy digital twin) | Simulated picker + order flow with KPIs |
| 9–12 | RL model development (state, action, reward design) | Prototype RL agent, training environment |
| 13–15 | RL training & tuning (Q-learning / DQN) | Trained RL agent, preliminary results |
| 16–18 | Experiments: RL vs heuristics | Comparative metrics (meters walked, time/order) |
| 19–20 | Evaluation, error analysis, improvements | Refined model + reflections |
| 21–22 | Draft final report & presentation prep | Draft report, figures, and demo material |
| 23 | 360° feedback + portfolio updates | Feedback report + reflection |
| 24 | Final submission & defense | Final report, portfolio, presentation |

---

## Part 2 – The Learning Activities

### 2a. Personal Learning Activities
- **360° Feedback**: I will ask for feedback at least twice from my coach, AI experts, and warehouse staff, focusing on my personal learning objectives.  
- **Self-reflection**: After feedback, I will reflect on my growth in AI application, system design, and project management. This includes evaluating if I have become more structured in research and more confident in applying AI to real-world cases.

### 2b. Theoretical Learning Activities (Learning Activity Reports)
For each learning activity, I will provide a **Learning Activity Report (L.A.R.)** including:
- **Preparations**: Expectations, related learning objectives, chosen methods.  
- **Content**: Summary of what was done, key findings.  
- **Conclusions**: Reflection on results, relation to objectives, possible new directions.

Planned L.A.R.s:
1. Literature study on RL and warehouse optimization.  
2. Baseline algorithm implementation (OR-Tools).  
3. Digital twin simulation setup.  
4. RL agent development and training.  
5. Experimental evaluation of RL vs. heuristics.  
6. Final results, analysis, and conclusions.  

---

## Appendix
- Literature list (to be filled during research).  
- Additional notes and datasets.  
