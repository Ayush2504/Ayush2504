<!--
  GitHub Profile README for Ayush Soni.
  ZERO GitHub Actions / scheduled workflows — every visual below is either a
  stateless hosted image URL (capsule-render, readme-typing-svg, shields.io)
  or plain Markdown/HTML. Nothing here ever needs a commit to stay current.

  Brand tokens pulled from index.html:92-93 — violet #8B5CF6, cyan #22D3EE,
  bg #070B14 — so this matches the portfolio exactly, not a generic theme.

  v3 fix: the header banner previously used capsule-render's `type=waving`,
  which draws its gradient via an SVG <animate> that starts from an EMPTY
  path ("d=\"\"") and only fills in once the animation begins. Any renderer
  that grabs a frame before that first tick (a slow load, GitHub's image
  cache, a link-preview bot) shows a blank/broken sliver instead of the
  gradient — confirmed by fetching the raw SVG and rendering it standalone.
  Switched to `type=rect`, which bakes the full gradient into a static
  <path> with no animation dependency — verified full-bleed on both light
  and dark backgrounds. Never use an animated-fill capsule-render type for
  a profile banner; static types only.

  Placeholders to fill in before publishing (search for ⟦):
    ⟦GITHUB_USERNAME⟧  — must exactly match this repo's name to render on your profile
    ⟦LINKEDIN_HANDLE⟧  — your LinkedIn public profile slug
    ⟦EMAIL⟧            — an email you're comfortable publishing
    ⟦RESUME_URL⟧       — direct link to a hosted PDF (Drive/Dropbox share link, or
                          host it on the portfolio and link there)
    ⟦CERT_VERIFY_URL_*⟧ — Microsoft Learn / Credly verification link per cert
                          (leave the badge but drop the href if you'd rather
                          not publish direct verify links — your call)

  Manually bump the "Last updated" line near the bottom every few months —
  there's no Action doing it for you, and a stale-looking date undercuts an
  otherwise-current page more than no date at all.
-->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:8B5CF6,100:22D3EE&height=180&section=header&text=Ayush%20Soni&fontSize=48&fontColor=F1F5F9&animation=fadeIn&fontAlignY=40&desc=Dynamics%20365%20CRM%20%26%20Power%20Platform%20Architect%20%C2%B7%20AI%20Solutions%20Engineer&descAlignY=68&descSize=18" width="100%" alt="Ayush Soni" />

<a href="https://ayushsoni25.com">
  <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=20&duration=3000&pause=1000&color=22D3EE&center=true&vCenter=true&width=600&lines=Dynamics+365+CRM+%26+Power+Platform+Architect;AI+Agent+Engineering+%C2%B7+RAG+%C2%B7+Copilot+Studio;Senior+Associate+%40+PwC+%C2%B7+8x+Microsoft+Certified" alt="Typing SVG" />
</a>

<img src="https://img.shields.io/badge/Available%20for-D365%20%2F%20Power%20Platform%20%2F%20AI%20collaborations-22D3EE?style=flat-square&labelColor=8B5CF6" alt="Available for collaborations" />

<p>
  <a href="⟦RESUME_URL⟧"><img src="https://img.shields.io/badge/Resume-Download-F1F5F9?style=for-the-badge&logo=readdotcv&logoColor=8B5CF6" alt="Resume" title="Download resume PDF" /></a>
  <a href="https://ayushsoni25.com"><img src="https://img.shields.io/badge/Portfolio-ayushsoni25.com-8B5CF6?style=for-the-badge&logo=googlechrome&logoColor=22D3EE" alt="Portfolio" title="Full case studies & impact log" /></a>
  <a href="https://linkedin.com/in/⟦LINKEDIN_HANDLE⟧"><img src="https://img.shields.io/badge/LinkedIn-Connect-8B5CF6?style=for-the-badge&logo=linkedin&logoColor=22D3EE" alt="LinkedIn" /></a>
  <a href="mailto:⟦EMAIL⟧"><img src="https://img.shields.io/badge/Email-Reach%20out-8B5CF6?style=for-the-badge&logo=gmail&logoColor=22D3EE" alt="Email" /></a>
</p>

</div>

<br />

```
$ whoami
ayush-soni · senior associate @ pwc

$ cat about.json
{
  "role": "Senior Associate, Dynamics 365 CRM & AI Solutions",
  "company": "PwC",
  "location": "⟦CITY, COUNTRY⟧",
  "open_to_relocation": ⟦true/false⟧,
  "experience": "5+ years",
  "certifications": 8,
  "focus": ["D365 CRM", "Power Platform", "Azure", "AI Agent Engineering"],
  "currently_exploring": ["Cloud Solution Architect", "AI Engineering roles"]
}
```

I architect enterprise **Dynamics 365 CRM & Power Platform** systems, and increasingly build the **AI layer on top of them** — Copilot Studio agents, RAG-grounded chatbots, and orchestrator agents that coordinate specialised sub-agents for review, testing, and QA. I bring the same AI-first approach into my own workflow too: Cursor- and Claude-driven test generation, PR-review agents, and `skill.md` files that teach coding agents my team's conventions.

**Note on this profile:** most of my production work lives in private enterprise/client repositories, not here — this page is a summary, not my activity feed. For real case studies and the full story, see **[ayushsoni25.com](https://ayushsoni25.com)**.

<br />

<div align="center"><sub>Where the AI work actually sits — not a replacement for the D365/Power Platform/Azure foundation, an extra layer on top of it.</sub></div>

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'primaryColor': '#8B5CF6', 'primaryTextColor': '#F1F5F9', 'primaryBorderColor': '#22D3EE', 'lineColor': '#22D3EE', 'secondaryColor': '#070B14', 'tertiaryColor': '#070B14'}}}%%
flowchart TB
    subgraph AI["🤖 AI Layer — increasingly built on top"]
        direction LR
        A1[Copilot Studio Agents]
        A2[RAG Chatbots]
        A3[Orchestrator & Sub-Agents]
    end
    subgraph CORE["🏗️ Core Specialization — the foundation, 5+ years"]
        direction LR
        F1[Dynamics 365 CRM]
        F2[Power Platform]
        F3[Azure]
    end
    CORE --> AI
```

<br />

<details open>
<summary><b>⚡ AI Engineering Highlights</b> — <i>click to expand</i></summary>
<br />

```diff
+ Built and deployed AI agents on Adobe's internal Cognito platform,
+ grounding conversational responses in live application data.

+ Designed a RAG-powered chatbot grounded in personalised, user-specific
+ data — keeping responses accurate to each user's own context.

+ Built an orchestrator agent coordinating specialised sub-agents
+ (review, test generation, QA) into one managed workflow.

+ Built an automated PR-review agent that flags convention drift
+ before a human reviewer looks.

+ Introduced a Cursor- and Claude-powered testing workflow that
+ auto-generates test cases straight from code changes.

+ Redesigned enterprise approval frameworks, reducing processing
+ time by ~35%.
```

**→ [Full case studies & impact log on the portfolio](https://ayushsoni25.com/#impact)**

</details>

<br />

### 🧩 How the orchestrator agent works

<sub>One diagram beats a paragraph of claims — this is the actual shape of the multi-agent workflow referenced above.</sub>

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'primaryColor': '#8B5CF6', 'primaryTextColor': '#F1F5F9', 'primaryBorderColor': '#22D3EE', 'lineColor': '#22D3EE', 'secondaryColor': '#22D3EE', 'tertiaryColor': '#070B14'}}}%%
flowchart LR
    A[Code change / PR opened] --> B{Orchestrator Agent}
    B --> C[Test-Generation Agent]
    B --> D[PR-Review Agent]
    B --> E[QA Scenario Agent]
    C --> F[Auto-generated test cases]
    D --> G[Convention & edge-case flags]
    E --> H[QA scenarios from code diff]
    F --> I[Managed workflow output]
    G --> I
    H --> I
```

<br />

<details>
<summary><b>🏗️ Core Specialization — D365, Power Platform & Azure</b> — <i>click to expand</i></summary>
<br />

```diff
+ Built real-time SAP ↔ D365 CRM synchronization ensuring data
+ consistency across systems.

+ Converted complex Power Automate flows into optimized C# plugins
+ for better performance and maintainability.

+ Developed a Flow Monitoring System for error tracking — received
+ client recognition.

+ Created a WhatsApp-integrated CRM enabling 2-way customer
+ communication.

+ Delivered a Canvas App spanning 30+ screens with complex,
+ maintainable architecture.

+ Implemented Azure DevOps pipelines, GitHub Actions and Jenkins
+ CI/CD for continuous integration and deployment.
```

**→ [Full case studies & impact log on the portfolio](https://ayushsoni25.com/#impact)**

</details>

<br />

### 🎯 Signature build — client project-closure automation

| | |
|---|---|
| **Problem** | Manual, multi-entity project closure with no way to validate readiness before committing — slow, error-prone, hard to audit. |
| **Approach** | Automated live data validation, built a pass/fail readiness dashboard, and orchestrated multi-entity closure end-to-end. |
| **Stack** | Power Platform · Dynamics 365 · Cursor AI · Claude · Copilot |
| **Outcome** | Turned a manual, multi-step closure process into a validated, repeatable one — accelerating delivery for the client. |

<br />

### 🛠️ Stack

<p>
  <img src="https://img.shields.io/badge/Dynamics_365-8B5CF6?style=flat-square&logo=microsoftdynamics365&logoColor=F1F5F9" title="Enterprise CRM architecture & plugin development" />
  <img src="https://img.shields.io/badge/Power_Platform-8B5CF6?style=flat-square&logo=powerapps&logoColor=F1F5F9" title="Canvas Apps, Power Automate, Power Pages" />
  <img src="https://img.shields.io/badge/Azure-22D3EE?style=flat-square&logo=microsoftazure&logoColor=070B14" title="Functions, Logic Apps, DevOps pipelines" />
  <img src="https://img.shields.io/badge/C%23-8B5CF6?style=flat-square&logo=csharp&logoColor=F1F5F9" title="Custom plugins & workflow extensions" />
  <img src="https://img.shields.io/badge/TypeScript-22D3EE?style=flat-square&logo=typescript&logoColor=070B14" title="Front-end tooling & automation scripts" />
  <img src="https://img.shields.io/badge/SQL-8B5CF6?style=flat-square&logo=microsoftsqlserver&logoColor=F1F5F9" title="Data modeling & integration queries" />
  <br />
  <img src="https://img.shields.io/badge/Copilot_Studio-22D3EE?style=flat-square&logo=microsoft&logoColor=070B14" title="Generative-AI features embedded in CRM workflows" />
  <img src="https://img.shields.io/badge/RAG-8B5CF6?style=flat-square&logo=openai&logoColor=F1F5F9" title="Retrieval-augmented chatbots grounded in user-specific data" />
  <img src="https://img.shields.io/badge/Multi--Agent_Orchestration-22D3EE?style=flat-square&logo=robotframework&logoColor=070B14" title="Orchestrator agent coordinating review, test-gen & QA sub-agents" />
  <img src="https://img.shields.io/badge/Cursor-8B5CF6?style=flat-square&logo=cursor&logoColor=F1F5F9" title="AI-assisted development workflow" />
  <img src="https://img.shields.io/badge/Claude-22D3EE?style=flat-square&logo=anthropic&logoColor=070B14" title="AI-assisted development workflow" />
</p>

<br />

### 🎓 Certifications — 8x Microsoft Certified

<p>
  <a href="⟦CERT_VERIFY_URL_PL900⟧"><img src="https://img.shields.io/badge/PL--900-Power_Platform_Fundamentals-8B5CF6?style=flat-square" /></a>
  <a href="⟦CERT_VERIFY_URL_MB910⟧"><img src="https://img.shields.io/badge/MB--910-D365_CRM_Fundamentals-8B5CF6?style=flat-square" /></a>
  <a href="⟦CERT_VERIFY_URL_PL400⟧"><img src="https://img.shields.io/badge/PL--400-Power_Platform_Developer-8B5CF6?style=flat-square" /></a>
  <a href="⟦CERT_VERIFY_URL_AZ900⟧"><img src="https://img.shields.io/badge/AZ--900-Azure_Fundamentals-8B5CF6?style=flat-square" /></a>
  <br />
  <a href="⟦CERT_VERIFY_URL_PL200⟧"><img src="https://img.shields.io/badge/PL--200-Power_Platform_Functional_Consultant-22D3EE?style=flat-square" /></a>
  <a href="⟦CERT_VERIFY_URL_MB230⟧"><img src="https://img.shields.io/badge/MB--230-Customer_Service_Functional_Consultant-22D3EE?style=flat-square" /></a>
  <a href="⟦CERT_VERIFY_URL_AZ204⟧"><img src="https://img.shields.io/badge/AZ--204-Developing_Solutions_for_Azure-22D3EE?style=flat-square" /></a>
  <a href="⟦CERT_VERIFY_URL_AB900⟧"><img src="https://img.shields.io/badge/AB--900-Copilot_%26_Agent_Admin_Fundamentals-22D3EE?style=flat-square" /></a>
</p>

<br />

<div align="center">
<i>Open to Dynamics 365, Power Platform & AI Engineering collaborations.</i>
<br />
<a href="https://ayushsoni25.com">ayushsoni25.com</a> · <a href="mailto:⟦EMAIL⟧">⟦EMAIL⟧</a>
<br /><br />
<sub>Last updated: August 2026</sub>
</div>
