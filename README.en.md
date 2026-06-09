<h1 align="center">Casey Lavier</h1>

<p align="center">
  <b>Systems administrator · Fullstack engineer</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/open_to-work-22c55e?style=flat-square" alt="open to work" />
  <img src="https://img.shields.io/badge/open_to-projects-0EA5E9?style=flat-square" alt="open to projects" />
  <img src="https://img.shields.io/badge/based_in-Moscow-64748b?style=flat-square" alt="based in Moscow" />
  <a href="https://t.me/CaseyLav"><img src="https://img.shields.io/badge/Telegram-%40CaseyLav-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Telegram @CaseyLav" /></a>
</p>

<p align="center">
  <sub><a href="./README.md">← Читать на русском</a></sub>
</p>

<hr/>

<p>
<b>I work across two adjacent disciplines — systems administration and fullstack development.</b> For the past four-plus years I've been responsible for production at the Russian State Children's Library: holding SLA 99.9%, running monitoring, CI/CD and runbooks, and leading a two-person IT team. Over the last six months I've shipped five fullstack applications to my own VPS, with health-gated deploys, automatic rollback and pre-deploy backups.
</p>

<p>
In parallel I'm finishing a bachelor's degree in Applied Informatics (Artificial Intelligence and Data Analysis) at Vitte Moscow University; I have a published paper on ML-based diagnosis of cardiovascular disease.
</p>

<h2>Tech stack</h2>

<table>
  <tr>
    <td width="22%"><b>Backend</b></td>
    <td>PHP 8.4 / Laravel 12 &nbsp;·&nbsp; Python / FastAPI &nbsp;·&nbsp; Go &nbsp;·&nbsp; Connect-RPC</td>
  </tr>
  <tr>
    <td><b>Frontend</b></td>
    <td>TypeScript &nbsp;·&nbsp; React 19 &nbsp;·&nbsp; Next.js 16 &nbsp;·&nbsp; Three.js &nbsp;·&nbsp; Tailwind</td>
  </tr>
  <tr>
    <td><b>Infrastructure</b></td>
    <td>Docker &nbsp;·&nbsp; GitHub Actions &nbsp;·&nbsp; Caddy &nbsp;·&nbsp; Nginx &nbsp;·&nbsp; Prometheus &nbsp;·&nbsp; Grafana</td>
  </tr>
  <tr>
    <td><b>Data &amp; ML</b></td>
    <td>PostgreSQL &nbsp;·&nbsp; MySQL &nbsp;·&nbsp; Redis &nbsp;·&nbsp; TensorFlow &nbsp;·&nbsp; scikit-learn</td>
  </tr>
</table>

<h2>Projects</h2>

<h3>Production — live on my own VPS <a href="https://lavier.tech">lavier.tech</a></h3>

<table>
  <thead>
    <tr>
      <th align="left">Project</th>
      <th align="left">Stack</th>
      <th align="left">What it is</th>
      <th align="left">Live</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b><a href="https://github.com/laviercasey/cosmos-explorer">cosmos-explorer</a></b></td>
      <td>Next.js 15 · React 19 · Three.js · Go · Connect-RPC · Postgres 16</td>
      <td>Interactive 3D model of the Solar System with a space-missions encyclopedia. 281 SSG pages, tag-based ISR with warm-up, Connect-RPC instead of REST, a throwaway build-time environment in CI that runs the SSG build against a live API.</td>
      <td><a href="https://cosmos.lavier.tech">cosmos.lavier.tech</a></td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/med-reminder-bot">med-reminder-bot</a></b></td>
      <td>FastAPI · aiogram · Celery · React</td>
      <td>Telegram Mini App for medication reminders. Transactional outbox with Celery delivery, JWT with refresh-token reuse detection, three-tier rate limiting, Redis Pub/Sub between services. Has real users.</td>
      <td><a href="https://t.me/MedNapominalkaBot">@MedNapominalkaBot</a></td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/Ecoshop">Ecoshop</a></b></td>
      <td>Laravel 12 · React 19 · FSD · Meilisearch</td>
      <td>Eco-goods e-commerce platform: 12 data models, 4-role RBAC, <code>lockForUpdate</code> guarding against checkout race conditions, Feature-Sliced Design enforced by Steiger in CI, PWA.</td>
      <td><a href="https://ecoshop.lavier.tech">ecoshop.lavier.tech</a></td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/portfolio-site">portfolio-site</a></b></td>
      <td>Next.js 16 · Go 1.25 · Postgres 16</td>
      <td>Bilingual personal-brand site. JSONB localization in the database, push-based ISR revalidation, singleflight cache in Go in front of the Umami API, health-gated deploy with auto-rollback via <code>.last-good-sha</code>.</td>
      <td><a href="https://lavier.tech">lavier.tech</a></td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/TicketHub">TicketHub</a></b></td>
      <td>PHP 8.4 · MySQL 8 · REST API</td>
      <td>Ticketing system: ~45-endpoint REST API, defense-in-depth (SHA-256 token hashing, brute-force and SSRF protection, CIDR allowlists), migrations with advisory locks. N+1 → JOIN optimization on the Kanban board: −99% queries.</td>
      <td><a href="https://tickethub.lavier.tech">tickethub.lavier.tech</a></td>
    </tr>
  </tbody>
</table>

<h3>Machine learning &amp; data</h3>

<table>
  <thead>
    <tr>
      <th align="left">Project</th>
      <th align="left">Stack</th>
      <th align="left">What it is</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b><a href="https://github.com/laviercasey/heart-disease-ml-benchmark">heart-disease-ml-benchmark</a></b></td>
      <td>Python · CatBoost · scikit-learn</td>
      <td>Multicenter ML benchmark for cardiovascular-disease diagnosis (n = 1,904 patients, 8 algorithms, 6 databases). CatBoost ROC-AUC <b>0.948</b> with BCa bootstrap confidence intervals and DeLong tests. Code for a published paper.</td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/metropt-predictive-maintenance">metropt-predictive-maintenance</a></b></td>
      <td>Python · GradientBoosting</td>
      <td>Early air-leak detection in a metro-train air compressor. ROC-AUC <b>0.9934</b>, F1 0.878 over 1.5 million time-series points (MetroPT-3 dataset, UCI).</td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/GenreNeuro">GenreNeuro</a></b></td>
      <td>TensorFlow · Keras</td>
      <td>Neural classifier of children's-book genres from text descriptions. Six genres, accuracy <b>89%</b> (+58.9% over baseline).</td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/Children-book-dataset">Children-book-dataset</a></b> &nbsp;·&nbsp; <b><a href="https://github.com/laviercasey/Diafilm-Parts-Finder">Diafilm-Parts-Finder</a></b></td>
      <td>Python · BeautifulSoup · fuzzy matching</td>
      <td>Library-domain data tooling: the scraper-built dataset behind GenreNeuro, and systematization of an unstructured filmstrip ("diafilm") database (regular expressions + fuzzy matching → Excel report on series and duplicates).</td>
    </tr>
  </tbody>
</table>

<h2>Education</h2>

<table>
  <tr>
    <td valign="top" width="18%"><b>2026</b></td>
    <td>BSc, Vitte Moscow University — <i>Applied Informatics (Artificial Intelligence and Data Analysis)</i>. Hands-on ML coursework throughout the program: building, training and evaluating models on real datasets.</td>
  </tr>
  <tr>
    <td valign="top"><b>2026</b></td>
    <td>karpov.courses — <i>System Analyst</i>. Requirements engineering, business-process modelling (BPMN, UML), REST API design, SQL, stakeholder communication.</td>
  </tr>
  <tr>
    <td valign="top"><b>2021</b></td>
    <td>Moscow State Educational Complex (MGOK) — <i>Network and System Administration</i>. Three-year programme: TCP/IP and OSI, routing, Windows Server and Linux administration.</td>
  </tr>
</table>

<h2>Publications</h2>

<ul>
  <li><b>"Comparative analysis of machine-learning algorithms for cardiovascular-disease diagnosis on a multicenter sample"</b> — C. M. Lavier. Code and data for reproduction: <a href="https://github.com/laviercasey/heart-disease-ml-benchmark">heart-disease-ml-benchmark</a>. CatBoost ROC-AUC 0.948, n = 1,904, 8 algorithms, 6 databases.</li>
</ul>

<h2>Production engineering — Russian State Children's Library, 4+ years</h2>

<ul>
  <li><b>SLA 99.9%</b> on a Prometheus + Grafana stack; production services running 24/7.</li>
  <li><b>MTTR reduced by 30%</b>, time-to-diagnosis by 25% after redesigning the network infrastructure from scratch.</li>
  <li><b>20+ production scripts</b> in Python and Bash: routine errors down 60%, ~15 team-hours saved per week.</li>
  <li><b>Deploy time cut from 2 hours to 15 minutes</b> by introducing CI/CD; no outages.</li>
  <li>Lead a two-person IT team and mentor a junior administrator.</li>
  <li>Technical audit and documentation of museum-space management systems — the organization no longer depends on its vendor.</li>
  <li>Knowledge base of 50+ articles: new-hire onboarding time cut from three weeks to one.</li>
</ul>

<h2>Freelance</h2>

<p>
Alongside my main role I take on fullstack engagements through word-of-mouth — bug-fixes, feature work and greenfield builds for small businesses, sole proprietors and private clients. Engagements range from one-off fixes of a few hours to multi-month builds.
</p>

<table>
  <tr>
    <td valign="top" width="22%"><b>Categories</b></td>
    <td>Maintenance and modernization of existing sites &nbsp;·&nbsp; new features and integrations (payment gateways, shipping, CRM, notifications) &nbsp;·&nbsp; greenfield builds &nbsp;·&nbsp; turn-key DevOps (VPS, SSL, Docker, CI/CD)</td>
  </tr>
  <tr>
    <td valign="top"><b>Stack</b></td>
    <td>Laravel &nbsp;·&nbsp; FastAPI &nbsp;·&nbsp; Next.js &nbsp;·&nbsp; React &nbsp;·&nbsp; PostgreSQL / MySQL &nbsp;·&nbsp; Docker &nbsp;·&nbsp; GitHub Actions &nbsp;·&nbsp; Caddy / Nginx &nbsp;·&nbsp; aiogram</td>
  </tr>
</table>

<p>
<sub>Most engagements run under verbal agreements in private client repositories; the public showcase of my stack is the open-source line above.</sub>
</p>

<h2>Contact</h2>

<ul>
  <li>Portfolio — <a href="https://lavier.tech">lavier.tech</a></li>
  <li>Telegram — <a href="https://t.me/CaseyLav">@CaseyLav</a></li>
  <li>Email — <a href="mailto:laviercasey@gmail.com">laviercasey@gmail.com</a></li>
</ul>
