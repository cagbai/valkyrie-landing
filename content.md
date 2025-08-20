# Valkyrie Landing Page Content

## 1) HERO — Banner
**Pre-header:** Run any AI model, any script, any workflow—without the infrastructure headache
**Headline:** Infinite Compute, On‑Demand. Introducing Valkyrie by Azumo.
**Paragraph:** Valkyrie by Azumo eliminates the biggest barrier to AI innovation: accessing scalable, optimized compute. Deploy LLMs, fine-tune models, generate content, or run custom workloads with a single API call.
**Primary CTA:** Request Early Access
**Secondary CTA:** See How It Works

## 2) The Pain — Bullet Checklist (fast empathy)
**Headline:** The Infrastructure Tax That's Killing Innovation
**Supporting:** Your team has brilliant ideas. Your models are ready. But you're stuck wrestling with GPU provisioning, environment setup, and cloud complexity instead of building what matters.

- **Weeks Lost to Setup:** Hunt for GPUs across providers. Debug environments that break in production. Fight fragile APIs and unclear errors. Your competitive advantage dies waiting for infrastructure.
- **Bleeding Money on Idle Resources:** Pay for clusters that sit unused. Overprovision for traffic spikes. Watch bills spiral while idle resources burn cash and you're still wrestling with basic setup.
- **Engineering Talent Wasted:** Your best developers become reluctant DevOps engineers. Security reviews slow every new tool addition. They're fixing infrastructure instead of solving problems.

## 3) How It Works — 4‑Step Timeline (visual flow)
**Pre‑header:** From API call to results—without the chaos
**Headline:** How Valkyrie Works
**Supporting paragraph:** You bring scripts, models, and data. Valkyrie provisions best‑fit compute (e.g., Vast.ai, RunPod, Hetzner, and others), manages dependencies, reports status clearly, and tears down cleanly when done.

**Content (timeline):**
1. **Submit** – Call a resilient REST endpoint with your job, artifacts, and params.
2. **Orchestrate** – Valkyrie provisions compute, installs requirements, loads models.
3. **Run & Report** – Status‑aware endpoints (queued, spinning up, loading, running, complete) with retries and reconciliation.
4. **Deliver & Clean Up** – Retrieve outputs or write to S3/GCS/Azure; environments auto‑terminate and are wiped.

## 4) What You Can Run — Card Grid (scannable)
**Pre‑header:** What You Can Run
**Headline:** One platform. Many possibilities.
**Supporting paragraph:** Use pre‑configured tools out of the box—or bring your own. If it's a script, Valkyrie will run it cleanly and at scale.

**Content (cards):**
- **Ollama (LLMs):** Chat, analysis, agents, custom apps
- **Unsloth (Fine‑tuning):** Efficient training on your data
- **Flux (Images):** Inpainting, outpainting, generative design
- **WAN 2.2 (Video):** AI‑driven video generation
- **Qwen‑Code:** "Vibe coding" for accelerated development
- **Bring Your Own:** Any Python/Unix script, model, or batch job

## 5) Use Case Spotlight — Split Layout (code + result box)
**Built For:** Engineering Teams Running Predictive Models
You've trained models. You need to run them at scale. Here's what that looks like when infrastructure isn't your problem.

**What You Bring:**
- Your Model: Trained XGBoost for pipeline flow prediction
- Your Data: CSV with thousands of scenarios to simulate
- Your Script: Simple Python runner for batch predictions

**What Valkyrie Does:**
```bash
curl -X POST "https://api.valkyrie.dev/instance/job/start" \
-H "X-API-Key: $YOUR_KEY" \
-d '{
  "cluster_name": "pipeline-predictions",
  "workdir": "~/models/pipeline_sim",
  "script": "python run_predictions.py --model model.json --data scenarios.csv"
}'
# Valkyrie handles: provisioning → execution → scaling → cleanup
```

**What You Get Back:**
- Predictions CSV: Flow rates for every scenario
- Minutes, Not Weeks: No infrastructure setup
- Pay Per Use: No idle cluster costs

**Perfect for:** Infrastructure Planning, Design Optimization, Risk Assessment
Run thousands of "what-if" scenarios without becoming a cloud expert. Focus on engineering decisions, not infrastructure management.

## 6) Business Value — Stat Bar (punchy, outcome‑led)
**Pre‑header:** Outcomes That Matter
**Headline:** Make infrastructure invisible. Make progress inevitable.
**Supporting paragraph:** Valkyrie compresses time‑to‑impact while keeping spend predictable and operations auditable.

- **Faster Innovation:** No more days lost configuring GPUs. Valkyrie provisions, runs, and scales compute in minutes so your team can focus on building, not setup.
- **Cost-Efficient by Design:** Automatic optimization across multiple providers. Auto-termination of idle clusters. Pay only for what you use, when you use it.
- **Enterprise-Grade Reliability:** Auto-scaling, GPU fallback, intelligent job scheduling, and robust authentication. Built for production from day one.
- **Simple Integration:** Intuitive REST APIs designed for resilience. Clear status reporting when models load, clusters spin up, or jobs execute.

## 7) Security & Compliance — Trust Boxes (reassurance section)
**Pre‑header:** Security & Compliance
**Headline:** Designed for privacy, auditability, and control
**Supporting paragraph:** Trust is foundational. Valkyrie bakes in controls that protect data, simplify reviews, and meet enterprise expectations—without slowing teams down.

- **Data Privacy First:** Customer data is never stored beyond job lifecycle. Fully abstracted and isolated workloads. Complete control over your proprietary information.
- **GDPR & Global Compliance:** Built-in data handling policies aligned with GDPR and international privacy regulations. Process sensitive data with complete confidence.
- **Ephemeral & Isolated:** Every compute instance is provisioned into an isolated environment. Automatic termination and data wiping when jobs complete.
- **Role-Based Access Control:** Fine-grained permissions ensure only authorized users and teams can access specific resources or endpoints.
- **Encrypted Communications:** All API requests secured with modern encryption protocols (TLS 1.2+). Support for both API keys and JWT tokens.
- **Audit Trail:** Detailed usage logs and wallet-based billing provide transparent records for internal governance and compliance reviews.

## 8) Why Valkyrie — Table (clarity at a glance)
**Pre‑header:** More Control, Less Friction
**Headline:** Better than DIY; more portable than single‑cloud
**Supporting paragraph:** DIY gives control but drains time. Single‑cloud is convenient until capacity or pricing shifts. Valkyrie is a unified execution fabric that's cost‑smart and portable.

| | DIY Orchestration | Single‑Cloud Runner | Valkyrie |
|---|---|---|---|
| Provisioning & Scale | Slow, manual | Easy until capacity/pricing shifts | Dynamic across providers |
| Cost Control | Idle burn common | Vendor‑dependent | Auto‑optimize + scale‑to‑zero |
| Portability | High effort | Low | High (open‑weight friendly) |
| Reliability | Brittle under growth | Varies by region/stock | Retries, reconciliation, failover |
| Security & Audits | Build it yourself | Mixed | Ephemeral, RBAC, audit logs |
| Dev Speed | Weeks to stable | Days | Minutes to first output |

## 10) Pricing & Early Access — Cards (commitment‑light)
**Pre‑header:** Early Access for teams ready to build
**Headline:** How To Get Started
**Supporting paragraph:** We're partnering with select teams to shape the roadmap in real environments. Access is commitment‑light and outcome‑focused.

**Content (cards):**

**Builder Teams** — For engineering‑led POCs and first production jobs
- Core platform access
- Pre‑configured tools (Ollama, Unsloth, Flux, WAN 2.2, Qwen‑Code)
- Email support, usage & cost visibility

**Scale & Enterprise** — For regulated, high‑throughput, or multi‑team workloads
- RBAC, audit logs, wallet‑based billing
- SSO/SAML (roadmap), VPC options (where applicable)
- Priority support, roadmap influence

**Primary CTA:** Request Early Access
**Secondary CTA:** Schedule a Call

## 11) Final CTA — Banner
**Headline:** Run any model. On any machine. With zero infrastructure drama.
**Primary CTA:** Get Early Access
**Secondary CTA:** Talk to an Engineer

## 12) FAQs — Accordion (objection handling)

1. **What types of models and workloads can I run on Valkyrie?** 
   Valkyrie can execute any script or model that runs in a containerized environment. This includes XGBoost, scikit-learn, PyTorch, TensorFlow models, custom Python/R scripts, data processing pipelines, and even non-ML workloads like simulations or batch analytics. If it runs on Linux, it runs on Valkyrie.

2. **How does pricing work? Am I paying for idle time?** 
   You only pay for actual compute time when your jobs are running. Valkyrie automatically terminates idle clusters, so there are no surprise bills from forgotten instances. Pricing is transparent and usage-based—you're billed per minute of actual execution time across our provider network.

3. **Where does my data go? Can I control data residency?** 
   Your data never leaves the isolated compute environment during job execution. All instances are ephemeral—completely wiped after job completion. For enterprise customers, we support deployment in your own cloud environment for complete data sovereignty and compliance with regional requirements.

4. **What happens if a job fails or gets interrupted?** 
   Valkyrie includes intelligent retry logic and reconciliation. If hardware fails, we automatically migrate your job to available resources. You get clear status reporting (queued, spinning up, running, failed, complete) so you always know what's happening. Failed jobs can be easily restarted without losing progress.

5. **How do I get my results back?** 
   Results can be retrieved directly through the API, automatically uploaded to your S3/GCS/Azure storage, or accessed through our secure download endpoints. You choose the method that fits your workflow—whether that's polling for completion or setting up webhooks for notifications.

6. **Is this just another wrapper around AWS/GCP?** 
   No. Valkyrie intelligently orchestrates across multiple providers (Vast.ai, RunPod, Hetzner, and others) to find the best price-performance for your specific workload. We handle provider failures, optimize routing, and abstract away the complexity of managing multiple cloud relationships.

7. **How quickly can I get started?** 
   If you have a working script and model, you can submit your first job within minutes of getting API access. No lengthy onboarding, no infrastructure setup, no DevOps expertise required. Our early access program includes direct support to help you optimize your first workflows.

8. **What about security and compliance? Can I get SOC 2?** 
   Valkyrie is built with enterprise-grade security from day one. We support GDPR compliance, provide detailed audit logs, use encrypted communications (TLS 1.2+), and offer role-based access control. SOC 2 certification is on our roadmap for enterprise customers.

9. **Can I integrate this with my existing MLOps pipeline?** 
   Yes. Valkyrie's REST API integrates seamlessly with existing tools like Airflow, Kubeflow, MLflow, or custom orchestration systems. You can treat Valkyrie as a compute backend that plugs into your current workflow without disrupting your established processes.

10. **What if I need specialized hardware or custom environments?** 
    Valkyrie automatically selects optimal hardware for your workload, including GPU-accelerated instances when needed. For custom environment requirements, you can specify dependencies in your job submission. Enterprise customers can work with us to pre-configure specialized environments for recurring use cases.