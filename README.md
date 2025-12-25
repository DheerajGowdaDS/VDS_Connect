# VDS Connect — Visual Agentic AI Pipeline Platform
![logo](https://github.com/DheerajGowdaDS/VDS_Connect/blob/main/assets/VDS.jpeg)

## Overview
**VDS Connect** is a developer-first, no-code platform for designing, deploying, and operating agentic AI pipelines.  
It enables teams to visually compose cognitive workflows using drag-and-drop nodes that represent stages like:

**Perception → Knowledge → Reasoning → Planning → Decision → Action → Learning**

The platform bridges the gap between model-centric experimentation and production-grade agent orchestration.  
It provides built-in messaging, state persistence, and execution control — allowing rapid prototyping, reproducible deployment, and closed-loop learning.

---

## Key Goals
- 🧩 Simplify orchestration of multi-node cognitive agents  
- 🔁 Enable reproducibility with per-node state persistence  
- 🚀 Accelerate deployment with secure API exposure and autoscaling  
- 🧠 Support learning loops with memory modules and feedback integration  
- 👩‍💻 Empower domain experts to build intelligent systems without writing glue code  

---

## Architecture Highlights

### System Components
| Layer         | Technology Stack | Role |
|--------------|------------------|------|
| Frontend      | React + TypeScript + React Flow | Visual pipeline builder and dashboard |
| Canvas Bridge | In-browser JS bridge | Local message routing and state updates |
| Backend API   | FastAPI (Python) | Node execution, metadata, file storage |
| Workers       | Docker containers (CPU/GPU) | Executes node logic and model inference |
| Message Bus   | Redis (Pub/Sub) | Fast message routing between nodes |
| Persistent DB | PostgreSQL | Stores pipeline manifests and node states |
| Object Store  | S3-compatible (MinIO/AWS) | Stores graphs, KR files, datasets |
| Observability | Prometheus + Grafana + PyVis | Logs, metrics, replay visualizations |
| Security      | JWT/OAuth, TLS, RBAC | Secure API access and multi-tenant isolation |

---

## Core Features
- **Visual Pipeline Builder** — drag-and-drop cognitive nodes with configuration panels  
- **Modular Node Templates** — Perception, Knowledge, Reasoning, Planning, Decision, Action, Learning  
- **State Persistence** — each node saves its state for reproducibility and debugging  
- **Execution Modes** — local preview, synchronous API, async job execution  
- **Connectors & Marketplace** — integrate external models, APIs, and datasets via plugins  
- **Observability & Replay** — queryable logs, saved outputs, and visual replay of pipeline runs  
- **Secure API Deployment** — export pipelines as REST endpoints with authentication and rate-limiting  
- **Learning & Memory Module** — capture experiences, retrain models, and update knowledge graphs  

---

## Cognitive Loop Design

![Cognitive Loop](https://github.com/DheerajGowdaDS/VDS_Connect/blob/main/assets/Cogni_loop.png)

---


- **Perception:** Ingest sensor data, images, text, or API inputs  
- **Knowledge + Reasoning:** Query ontologies, rules, and facts to infer new insights  
- **Planning + Decision:** Generate candidate plans and select optimal actions  
- **Action:** Execute commands, trigger APIs, or control actuators  
- **Learning:** Store experiences, evaluate outcomes, and update models or memory  

---

## Execution Flow
1. User designs pipeline in the visual builder  
2. Pipeline manifest saved to database  
3. Triggered via API or manual run  
4. Controller schedules node execution  
5. Workers run node logic and return outputs  
6. Outputs forwarded to downstream nodes  
7. Node states persisted for replay and debugging  
8. Final result returned to caller or stored in memory  

[▶️ Watch Demo Video](https://drive.google.com/file/d/1PLKhhRt8GJxyjkv1IwJktBkEiQF5pxnP/view?usp=sharing)

---

## Deployment Models
- **Local Development:** Docker Compose setup with FastAPI, Redis, Postgres, and local worker  
- **Production:** Kubernetes cluster with autoscaled worker pods, secure ingress, and monitoring stack  
- **API Exposure:** Each pipeline becomes a secure REST endpoint with per-tenant isolation  

---

## Example Use Cases
- 🌾 **Smart Agriculture:** Drone imagery → disease detection → spraying schedule → feedback loop  
- 🏥 **Medical Triage:** Patient data → reasoning → treatment planning → human-in-the-loop approval  
- 🤖 **Autonomous Robotics:** Sensor fusion → path inference → trajectory planning → motor control  
- 💬 **Customer Support Automation:** Multimodal input → knowledge graph reasoning → automated response  

---

## Competitive Landscape
- **LangChain / LlamaIndex:** Strong in LLM orchestration; VDS Connect adds multi-node cognitive flows  
- **aiXplain / PaaS providers:** Offer APIs; VDS Connect adds orchestration + knowledge integration  
- **NVIDIA (Isaac, Clara):** Focused on robotics; VDS Connect is domain-agnostic  
- **Google Vertex AI / AWS SageMaker:** Training/deployment platforms; VDS Connect emphasizes visual orchestration + reasoning  

---

## Innovation & Differentiators
- Knowledge-first architecture (ontologies, rules, procedural graphs)  
- Node-level persistence ensures reproducibility across runs  
- In-browser bridge for rapid iteration without backend deployment  
- Extensible marketplace for node plugins and datasets  
- Closed-loop learning integrated into pipeline lifecycle  
- Human-in-the-loop support for approvals and audit trails  

---

## Conclusion
**VDS Connect** transforms complex agentic AI systems into **composable, reproducible workflows**.  
It reduces engineering overhead, accelerates iteration, and enables production-grade deployment.  
The vision: a unified platform where teams can design, deploy, and continuously improve intelligent agents with ease.

---

## 👨‍💻 Team Contacts
```bash
echo "Reach out to us:"
echo "Dheeraj Gowda D S  | Discord: dheerajgowda_ds_03916 | Mail: dsdheeraj70@gmail.com"
echo "Sagar T K | Mail: sagartktmd@gmail.com
echo "Vrunda S | Mail: vrundareddy1664@gmail.com"
