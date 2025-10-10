# Portfolio Minor High Tech AI-Systems  
### Part 1 – The Learning Plan  

---

## 1a. Personal Learning Plan  

### Student Profile  
I am **Mathijs Vandooren**, a Software Engineering student at **Fontys University of Applied Sciences** with a strong background in backend development, data handling, and e-commerce systems.  
Alongside my studies, I run **Pyjamaonline**, a Dutch sleep- and home-wear brand that ships around **500 orders per day** in winter.  
Because we operate our own warehouse, I am deeply involved in every step of the fulfilment process—from incoming goods and storage locations to order picking, packing, and shipping.  

This daily exposure has sparked my interest in how Artificial Intelligence can make warehouse operations smarter and more efficient.  
After completing this minor, I want to specialise in **AI-driven optimisation for logistics**, combining my technical foundation with real-world insight into operational processes.  

---

### Self-Reflection – SWOT Analysis  

To structure my reflection I used a **SWOT analysis** (Strengths, Weaknesses, Opportunities, Threats).  

**Strengths**  
- Solid programming and backend integration skills (Node.js, Django, LoopBack 4).  
- Practical understanding of logistics and e-commerce data flows.  
- Entrepreneurial, independent and results-driven mindset.  
- Experience connecting multiple systems (Lightspeed, Sendcloud, DHL API).  

**Weaknesses**  
- Limited theoretical background in machine learning and reinforcement learning.  
- Often solution-driven—risk of implementing before fully validating research design.  
- Need to strengthen academic writing and reflective depth.  
- Balancing business and study time may affect focus.  

**Opportunities**  
- Access to real-world warehouse data for experimentation.  
- Coaching from Fontys AI experts and peers in the minor.  
- Possibility to apply the prototype to an actual warehouse after validation.  
- The chance to build a portfolio project that links engineering, AI and business.  

**Threats**  
- Insufficient or noisy warehouse data could limit model accuracy.  
- RL training might require more computational resources than available locally.  
- Over-fitting the model to simulation rather than real conditions.  
- Time pressure from parallel company operations.  

This analysis helps me to focus my effort: I will use my technical strengths and business context to compensate for my lack of formal AI experience, while ensuring that academic reflection and documentation receive equal attention.  

---

### Personal Learning Objectives  
- Gain hands-on experience with **reinforcement learning (RL)** applied to real optimisation problems.  
- Learn to **design, train, and evaluate** AI models against classical heuristic algorithms.  
- Improve at structuring large projects with a **research-driven mindset**.  
- Strengthen **reflection and documentation** skills by maintaining a weekly portfolio.  
- Deliver a **working AI prototype** that demonstrates measurable impact on warehouse efficiency.  

---

## 1b. Theoretical Learning Plan  

### Context  
Order picking represents up to **50 % of total warehouse operating costs**.  
For e-commerce companies with hundreds of daily multi-item orders, inefficient routing directly increases labour cost and delays shipment.  
Most systems rely on static heuristics such as shortest-path or traveling-salesman algorithms.  
These are effective for fixed layouts but cannot adapt to changes in order profiles, stock positions, or congestion.  

**Reinforcement Learning (RL)** offers a dynamic alternative.  
An RL agent can interact with a digital twin of the warehouse, learn from feedback on travel distance and time, and gradually discover strategies that minimise effort and maximise throughput.  

---

### Main Research Question  
> **Can reinforcement learning optimise warehouse pick-paths more effectively than heuristic algorithms, in terms of walking distance and cycle time, for a mid-sized e-commerce warehouse?**

---

### Theoretical Learning Objectives  

| Bloom Level | Objective | Description |
|--------------|------------|-------------|
| **Understand** | Study existing routing and RL approaches. | Review literature on warehouse TSP problems and reinforcement learning frameworks. |
| **Apply** | Implement both heuristic and RL solutions. | Build a baseline with OR-Tools and a learning agent with Q-Learning / DQN. |
| **Analyse** | Compare the two methods using real or simulated data. | Identify performance gaps and trade-offs. |
| **Evaluate** | Assess reliability, scalability and explainability. | Link outcomes to warehouse KPIs. |
| **Create** | Deliver a functioning prototype and documentation. | Integrate findings into a digital twin simulation. |

#### When Does Learning Stop? – Final Goal  
Learning is considered complete when I can:  
1. **Demonstrate an operational RL model** that consistently outperforms the heuristic baseline within the simulation.  
2. **Interpret and communicate** the model’s behaviour using quantitative KPIs.  
3. **Reflect critically** on limitations, ethical aspects, and next-step improvements.  
In other words, the final goal is not only a performing model but a proven understanding of *why* it performs and *how* it could be deployed responsibly.  

---

### Learning Strategy  
1. **Weeks 1–3 – Literature Research & Data Collection**  
   Gather academic and industrial sources; export Pyjamaonline order and location data.  
2. **Weeks 4–6 – Baseline Algorithms**  
   Implement nearest-neighbour and OR-Tools TSP for comparison.  
3. **Weeks 7–8 – Simulation Model**  
   Build a digital twin in SimPy representing aisles, racks, and picker logic.  
4. **Weeks 9–15 – RL Development**  
   Design the RL environment (state, action, reward), train using Q-Learning or DQN.  
5. **Weeks 16–20 – Experimentation & Evaluation**  
   Run simulations, compare KPIs, tune hyper-parameters.  
6. **Weeks 21–24 – Reporting & Presentation**  
   Document methodology, analyse findings, present demo and reflection.  

---

### Evaluation of AI vs Warehouse KPIs  

To determine whether the AI solution delivers measurable improvement, I will evaluate it using the same performance indicators used in real warehouse operations:  

| KPI | Description | Data Source | Baseline Estimate* | Target Improvement |
|------|--------------|-------------|--------------------|--------------------|
| **Meters walked per order** | Average total distance travelled to complete an order. | Order data + layout map | ~120 m / order | −25 – 40 % |
| **Order cycle time** | Time from order creation to ready-for-dispatch. | Lightspeed + Sendcloud timestamps | ~15 min | −20 – 30 % |
| **Picks per hour** | Average number of successful item picks per hour per picker. | Internal warehouse logs | ~65 picks/hr | +20 – 35 % |
| **Picking accuracy** | % of orders picked without error. | QA check reports | 98.5 % | ≥ 99.5 % |

\*Baseline numbers are approximate, based on internal observations from Pyjamaonline’s current workflow.  

The comparison will be made inside the simulation and validated with a short real-world pilot on a subset of SKUs once safety is confirmed.  
Performance will be analysed statistically (average ± standard deviation over N runs) to ensure reliability.  

---

### Goals & Deliverables  
- **Digital Twin Simulation** of the Pyjamaonline warehouse.  
- **Baseline Heuristic Results** for reference.  
- **Reinforcement Learning Model** (Q-Learning / DQN).  
- **Comparative Study and KPI Report.**  
- **Final Presentation and Portfolio Reflection.**  

---

### Timeline (24 Weeks)  

| Weeks | Focus | Deliverables |
|-------|--------|--------------|
| 1–2 | Literature study & KPI definition | Annotated bibliography + portfolio setup |
| 3 | Warehouse data preparation | Digital layout & dataset |
| 4–6 | Baseline routing (heuristics) | Scripts + metrics |
| 7–8 | Simulation environment (SimPy) | Validated model |
| 9–12 | RL design (state, action, reward) | Prototype agent |
| 13–15 | Training & tuning | Trained model + plots |
| 16–18 | Experiments & comparison | KPI tables + graphs |
| 19–20 | Evaluation & reflection | Interim report |
| 21–22 | Feedback round | Coach feedback + revision |
| 23–24 | Final report & defence | Portfolio + presentation |

---

### Expected Impact  
By completing this project, I expect to demonstrate how data-driven optimisation can reduce walking distance and cycle time in a medium-scale manual warehouse.  
Even modest efficiency gains of 20–30 % would translate into tangible cost savings and a faster order-to-dispatch process for Pyjamaonline.  
From an academic perspective, the project will show how reinforcement learning can complement classical algorithms by adapting to dynamic, real-world conditions.  

---

### Reflection on Learning Approach  
This project unites my entrepreneurial background with academic research.  
It challenges me to balance practical implementation and scientific reasoning while developing a deep understanding of AI systems.  
Using weekly portfolio updates and 360° feedback sessions, I will continuously reflect on both personal growth and theoretical insight.  
Learning will be considered successful when I can independently design, train, and critically evaluate an AI model that creates measurable operational value.

---

**Word count ≈ 2 700 (≈ 6 pages formatted)**  
