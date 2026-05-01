#  DispatchCTRL – Fair AI Route Dispatch System  
### *(RouteConscience: Human-Style Fair Dispatch Engine)*

---

##  Overview  

DispatchCTRL (RouteConscience) is a fairness-driven route dispatch system designed to mimic how a thoughtful human dispatcher assigns delivery routes.  

Instead of blindly optimizing numerical values, the system reasons step-by-step, considering driver capability, workload history, preferences, and overall well-being.  

It ensures that:
- No driver is consistently overloaded  
- New drivers are protected  
- Assignments are transparent and explainable  

---

##  Problem Statement  

In real-world delivery systems, drivers often experience unequal workloads despite performing the same job.  

Examples:
- One driver may receive light packages in easy locations  
- Another may handle heavy deliveries with stairs and parking difficulties  
- Some drivers repeatedly get harder routes without explanation  

This creates dissatisfaction, fatigue, and lack of trust in automated systems.  

The goal is to build a system that assigns routes fairly while explaining decisions clearly, similar to a human dispatcher.

---

##  Solution  

RouteConscience introduces a constraint-based fairness dispatch system that:

- Evaluates route difficulty based on real-world effort  
- Considers driver attributes and preferences  
- Balances workload over time  
- Provides human-readable explanations for every decision  

---

##  Key Features  

- Fair workload distribution over time  
- Transport-aware route assignment  
- Age and physical suitability consideration  
- New driver onboarding with safe workload  
- Shift preference handling  
- End-of-day route optimization (closer to home)  
- Transparent and explainable decisions  

---

##  System Architecture  

<img width="1675" height="913" alt="image" src="https://github.com/user-attachments/assets/f0029677-ac99-4fd2-9c24-89d757f8d12f" />


---

##  Core Modules  

### Route Analysis Module  
Analyzes:
- Number of packages  
- Package weight  
- Delivery environment  
- Parking difficulty  

Outputs: Easy / Moderate / Hard / Very Hard  

---

### Driver Profile Module  
Stores:
- Transport type  
- Age category  
- Shift preference  
- Experience level  
- Home location  

---

### Workload History Module  
Tracks:
- Recent workload difficulty  
- Consecutive hard routes  
- Overall workload trends  

---

### Fairness Decision Engine  
Combines:
- Transport feasibility  
- Age suitability  
- Preferences  
- Experience level  
- Workload balance  
- End-of-day convenience  

---

### Explanation Generator  
Provides reasons such as:
- Assigned due to workload balance  
- Matched transport suitability  
- Adjusted based on recent heavy routes  
- Final delivery closer to home  

---

##  Dispatch Flow  

1. Transport feasibility check  
2. Age suitability adjustment  
3. Shift preference matching  
4. New driver onboarding check  
5. Workload fairness evaluation  
6. End-of-day destination consideration  
7. Final assignment with explanation  

---

##  Algorithm  

### Constraint-Based Fairness Ranking Algorithm  

Step 1: Apply hard constraints  
- Transport compatibility  
- Availability  

Step 2: Apply soft constraints  
- Age suitability  
- Shift preference  
- Experience level  
- End-of-day proximity  

Step 3: Rank drivers based on fairness  
- Using workload history  

Step 4: Assign route and generate explanation  

---

##  Tech Stack  

### Frontend  
- HTML5  
- CSS3  
- JavaScript  

### Backend  
- Python 3  
- Flask  

### Core Logic  
- Rule-based fairness engine  
- Fairness Load Index (FLI)  

### Data Storage  
- JSON  
- SQLite  

### AI (Explanation Only)  
- Ollama (Local LLM)  
- Models: LLaMA 3 / Mistral  

### RAG System  
- JSON/text-based retrieval for explanations  

---

##  How It Works  

1. Collect route and driver data  
2. Analyze and classify route difficulty  
3. Filter eligible drivers  
4. Apply constraints  
5. Rank drivers using fairness logic  
6. Assign route  
7. Generate explanation  
8. Update workload history  

---

##  Why This System is Different  

- Focuses on fairness, not just efficiency  
- Uses human-like reasoning instead of black-box models  
- Provides transparent and explainable decisions  
- Balances workload across multiple days  

---

##  Future Enhancements  

- Integration with live maps  
- Mobile application support  
- Real-time GPS tracking  
- Advanced analytics dashboard  
- Optional AI-based optimization layer  

---

##  Author  

DHEEKSHITA R 

---

