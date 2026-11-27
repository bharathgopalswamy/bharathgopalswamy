<p align="center">
  <img src="./assets/banner.svg" alt="Bharath Gopalsamy — Business Systems Developer and Application Support. I build and support the internal systems organizations run on: service desks, intake workflows, records and reporting." width="100%" />
</p>

<p align="center">
  <a href="https://service-desk-ticketing-system.onrender.com"><img src="https://img.shields.io/badge/Live_demo-Service_Desk-22D3EE?style=for-the-badge&logo=render&logoColor=white" alt="Service Desk live demo" /></a>
  <a href="https://bharathgopalsamy.vercel.app"><img src="https://img.shields.io/badge/Portfolio-0EA5E9?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio" /></a>
  <a href="https://linkedin.com/in/bharathgopalsamy"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:bharathgopalswamy09@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Nova_Scotia-Canada-0F766E?style=flat-square" alt="Nova Scotia, Canada" />
  <img src="https://img.shields.io/badge/MACS-St_Francis_Xavier_University-1E3A8A?style=flat-square" alt="Master of Applied Computer Science, StFX" />
  <img src="https://img.shields.io/badge/Open_to-full--time_roles_across_Canada-15803D?style=flat-square" alt="Open to full-time roles across Canada" />
</p>

---

### The problem space I work in

Most of what keeps an organization running isn't its public website. It's the **internal systems** behind it: the service desk that triages a broken laptop, the form that turns a maintenance report into a work order, the records system an admissions team lives in, and the reports a manager reads on Monday.

That's where my experience sits:

- **Building** those systems: React interfaces, Node.js/Express APIs, SQL data models, validation and tests.
- **Supporting** them: investigating defects, tracing API and state issues, regression checks, documenting fixes.
- **Using** them: I currently process applications and keep records accurate in a Salesforce-based CRM (TargetX) at StFX Admissions.

I'm looking for full-time roles as a **junior software developer, application / IT support analyst, or business systems analyst**.

---

### Systems map

My flagship projects are designed as parts of one operations platform. Each one is a complete, tested application on its own.

```mermaid
flowchart LR
    I["🛠️ Intake<br/><b>MaintainIQ</b><br/>free text → validated work request"]
    S["🎫 Service Desk<br/><b>Ticketing System</b><br/>priority · SLA · workflow · audit"]
    R["🗂️ Records<br/><b>Admissions Workflow</b><br/>Java · Spring Boot · PostgreSQL"]
    A["📊 Reporting<br/><b>IT Operations Analytics</b><br/>SQL · Power BI"]
    I -->|work requests| S
    S -->|ticket + SLA data| A
    R -.->|application funnel| A
    I -.->|structured exports| A
    classDef live fill:#0F172A,stroke:#22D3EE,color:#E2E8F0;
    classDef planned fill:#0F172A,stroke:#64748B,color:#94A3B8,stroke-dasharray:4 4;
    class I,S live;
    class R,A planned;
```

<sub>Solid = built and on GitHub · dashed = on the roadmap</sub>

---

### Flagship projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>🎫 Service Desk Ticketing System</h4>
      <a href="https://github.com/bharathgopalswamy/service-desk-ticketing-system"><img src="https://raw.githubusercontent.com/bharathgopalswamy/service-desk-ticketing-system/main/docs/screenshots/queue.png" alt="Service desk ticket queue with priority and live SLA countdown" width="100%" /></a>
      <p>IT service desk modelled on how internal support teams handle incidents.</p>
      <ul>
        <li>ITIL-style <b>impact × urgency → P1–P4</b> priority</li>
        <li>Response and resolution <b>SLA deadlines</b> with breach detection</li>
        <li>Server-enforced ticket <b>workflow</b> and full <b>audit trail</b></li>
        <li>SQL <b>reporting</b>: SLA compliance, breaches, resolution time</li>
        <li>39 automated tests · CI · Docker</li>
      </ul>
      <p><code>React</code> <code>Node.js</code> <code>Express</code> <code>SQLite</code> <code>Zod</code> <code>Vitest</code> <code>Docker</code></p>
      <p><a href="https://service-desk-ticketing-system.onrender.com"><b>Live demo</b></a> · <a href="https://github.com/bharathgopalswamy/service-desk-ticketing-system"><b>Source</b></a> · <a href="https://github.com/bharathgopalswamy/service-desk-ticketing-system/blob/main/docs/ARCHITECTURE.md"><b>Architecture</b></a></p>
    </td>
    <td width="50%" valign="top">
      <h4>🛠️ MaintainIQ Intake</h4>
      <p>Turns plain-language maintenance reports into structured CMMS work requests. A person reviews every field before anything is submitted.</p>
      <ul>
        <li>Gemini extraction validated against a <b>Zod schema</b>; unknown fields stay blank and are flagged, never invented</li>
        <li>Deterministic <b>safety rules</b> (gas, fire, electrical) escalate priority independently of the AI</li>
        <li>Safe error handling: internal details are logged, not shown to users</li>
        <li>Automated tests · CI · Docker</li>
      </ul>
      <p><code>React</code> <code>Express</code> <code>Gemini API</code> <code>Zod</code> <code>Vitest</code> <code>Docker</code></p>
      <p><a href="https://github.com/bharathgopalswamy/maintainiq-intake"><b>Source</b></a></p>
    </td>
  </tr>
</table>

<details>
  <summary><b>More projects</b> (data, full-stack, analytics)</summary>
  <br/>

| Project | What it shows | Stack | Links |
|---|---|---|---|
| **Job Market Reality Check** | Analysis of 2,253 data-analyst postings: skill demand with SQL (joins, CTEs, window functions) | Python · SQL · MySQL · Power BI | [Source](https://github.com/bharathgopalswamy/job-market-reality-check) |
| **Spotify Music Intelligence** | API → ETL → normalized MySQL → Power BI pipeline (10 albums, 124 tracks) | Python · Spotipy · MySQL · Power BI | [Demo](https://spotify-music-intelligence-platform.vercel.app) · [Source](https://github.com/bharathgopalswamy/Spotify-Music-Intelligence-Platform) |
| **DermaCure** | Role-based patient / doctor / admin workflows with JWT auth (portfolio prototype, not clinically validated) | React · Node.js · MongoDB · Docker | [Demo](https://derma-ai-psi.vercel.app) · [Source](https://github.com/bharathgopalswamy/DermaAI) |
| **HabitIQ** | TypeScript full-stack app with analytics dashboards and optional AI planning | React · TypeScript · Node.js · MongoDB | [Demo](https://habitiq-blond.vercel.app) · [Source](https://github.com/bharathgopalswamy/smart-ai-habit-tracker) |

</details>

---

### Experience

| Role | Where | What I do / did |
|---|---|---|
| **Admissions Assistant** | St. Francis Xavier University | Process applications and maintain applicant records in TargetX CRM; Excel reporting and data-quality checks |
| **Website Coordinator & Technical Support** | StFX | Improved a page's PageSpeed score from 32 to 93; fixed broken links and layout defects with DevTools; desktop/mobile QA |
| **Software Developer** | FirstLanguage Technologies | React + TypeScript features on REST APIs; defect investigation; functional and regression testing |
| **Frontend Developer Intern** | FirstLanguage Technologies | Reusable dashboard components with Context and custom hooks; API/state defect tracing |
| **ReactJS Developer Intern** | Banao Technologies | Wireframes → responsive forms, tables and dashboards; REST API integration |

---

### How I build

- **Tests first-class:** business rules (priority, SLA, workflow) are unit-tested; APIs are tested end to end with Supertest; UIs with React Testing Library.
- **CI on every change:** lint → tests → build → Docker build and smoke test, via GitHub Actions.
- **Decisions written down:** each flagship has an `ARCHITECTURE.md` (diagrams, data model, trade-offs) and a `DEVLOG.md`.
- **Validate on the server, guide in the UI:** the client only offers valid actions; the API still enforces them.
- **Open about tooling:** I use AI pair-programming (Claude Code) on portfolio projects. I define the requirements, review every pull request, and can explain every design decision.

---

### Toolbox

<p align="center">
  <img src="https://skillicons.dev/icons?i=react,ts,js,nodejs,express,python,mysql,sqlite,mongodb,docker,githubactions,git,postman,vite,tailwind&perline=15" alt="React, TypeScript, JavaScript, Node.js, Express, Python, MySQL, SQLite, MongoDB, Docker, GitHub Actions, Git, Postman, Vite, Tailwind" />
</p>

| Area | Tools |
|---|---|
| Application development | React, TypeScript, JavaScript, Node.js, Express, REST APIs, Zod |
| Data and reporting | SQL, MySQL, SQLite, MongoDB, Python, Excel, Power BI |
| Quality | Vitest, Jest, React Testing Library, Supertest, Postman, regression testing |
| Delivery | Git, GitHub Actions, Docker, Vercel, Render |
| Business systems | TargetX CRM (Salesforce-based), ITIL fundamentals, Microsoft Teams, SharePoint |

---

### Now building

- [ ] **Service Desk v0.3:** SLA clock pauses while On Hold · logins with requester / agent / lead roles · business-hours SLA
- [ ] **Admissions Application Workflow System:** Java 21, Spring Boot, PostgreSQL, JUnit; fictional data only
- [ ] **IT Operations Analytics:** a SQL star schema and Power BI report over the Service Desk and MaintainIQ data

---

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/bharathgopalswamy/bharathgopalswamy/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/bharathgopalswamy/bharathgopalswamy/output/github-contribution-grid-snake.svg" />
  <img alt="Contribution graph animation" src="https://raw.githubusercontent.com/bharathgopalswamy/bharathgopalswamy/output/github-contribution-grid-snake.svg" />
</picture>

<p align="center">
  <sub>Based in Nova Scotia · open to Atlantic Canada, remote within Canada, and relocation for the right role</sub>
</p>
