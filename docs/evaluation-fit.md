# Evaluation Fit

---

## Problem Relevance
Dangerous trucking due to climate and robbery is a real problem that affects drivers, logistics firms, and supply chains. This project keeps people out of harm while maintaining deliveries.

---

## Idea Feasibility
We demonstrate the concept with diagrams, a dashboard mockup, and a clear AI-in-the-loop workflow.  
It is realistic for a student team to build and iterate digitally without hardware.

---

## Use of OpenAI APIs
- **GPT:** Provides risk-aware routing advice in JSON.  
- **Whisper:** Enables hands-free emergency commands.  
- **Design Principle:** APIs are used thoughtfully as decision support, *not as direct actuators*.  

---

## Risk Assessment

| **Risk**                  | **Impact** | **Mitigation** |
|----------------------------|------------|----------------|
| Satellite link outage      | Loss of connectivity | Fallback to local autonomy until reconnect |
| LLM hallucination / error  | Unsafe route suggestion | Operator validation + secondary rule-based check |
| Cybersecurity attack       | Hijacked comms | Encryption, multi-factor auth, monitoring |
| Operator delay             | Slower response | Prioritize alerts, redundant staff shifts |
| Hardware failure (truck)   | Vehicle disabled | Standard roadside recovery protocols |

---

## Bottom Line
- Relevant: addresses urgent trucking safety issues  
- Feasible: can be prototyped digitally, scaled later  
- Responsible: AI used carefully, operator always in the loop  
