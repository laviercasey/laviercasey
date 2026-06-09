<h1 align="center">Кейси Лавьер</h1>

<p align="center">
  <b>Системный администратор · Fullstack-инженер</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/open_to-work-22c55e?style=flat-square" alt="open to work" />
  <img src="https://img.shields.io/badge/open_to-projects-0EA5E9?style=flat-square" alt="open to projects" />
  <img src="https://img.shields.io/badge/based_in-Moscow-64748b?style=flat-square" alt="based in Moscow" />
  <a href="https://t.me/CaseyLav"><img src="https://img.shields.io/badge/Telegram-%40CaseyLav-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Telegram @CaseyLav" /></a>
</p>

<p align="center">
  <sub><a href="./README.en.md">Read in English →</a></sub>
</p>

<hr/>

<p>
<b>Развита в двух направлениях — системное администрирование и fullstack-разработка.</b> Четыре с лишним года я отвечаю за production в Российской государственной детской библиотеке: держу SLA 99.9%, веду мониторинг, CI/CD и runbook'и, руковожу IT-командой из двух инженеров. За последние шесть месяцев на собственном VPS подняла пять fullstack-приложений — с health-gate деплоями, авто-rollback и pre-deploy backups.
</p>

<p>
Параллельно заканчиваю бакалавриат по прикладной информатике (искусственный интеллект и анализ данных) в Московском университете имени С.Ю. Витте; есть опубликованная научная статья по ML-диагностике сердечно-сосудистых заболеваний.
</p>

<h2>Технологии</h2>

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
    <td><b>Инфраструктура</b></td>
    <td>Docker &nbsp;·&nbsp; GitHub Actions &nbsp;·&nbsp; Caddy &nbsp;·&nbsp; Nginx &nbsp;·&nbsp; Prometheus &nbsp;·&nbsp; Grafana</td>
  </tr>
  <tr>
    <td><b>Данные и ML</b></td>
    <td>PostgreSQL &nbsp;·&nbsp; MySQL &nbsp;·&nbsp; Redis &nbsp;·&nbsp; TensorFlow &nbsp;·&nbsp; scikit-learn</td>
  </tr>
</table>

<h2>Проекты</h2>

<h3>Production — в проде на собственном VPS <a href="https://lavier.tech">lavier.tech</a></h3>

<table>
  <thead>
    <tr>
      <th align="left">Проект</th>
      <th align="left">Стек</th>
      <th align="left">Что это</th>
      <th align="left">Live</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b><a href="https://github.com/laviercasey/cosmos-explorer">cosmos-explorer</a></b></td>
      <td>Next.js 15 · React 19 · Three.js · Go · Connect-RPC · Postgres 16</td>
      <td>Интерактивная 3D-модель Солнечной системы и энциклопедия космических миссий. 281 SSG-страница, ISR с тегированной инвалидацией и прогревом, Connect-RPC вместо REST, throwaway-окружение в CI для прогона SSG-сборки против живого API.</td>
      <td><a href="https://cosmos.lavier.tech">cosmos.lavier.tech</a></td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/med-reminder-bot">med-reminder-bot</a></b></td>
      <td>FastAPI · aiogram · Celery · React</td>
      <td>Telegram Mini App для напоминаний о приёме лекарств. Транзакционный outbox с доставкой через Celery, JWT с reuse-detection refresh-токенов, трёхуровневый rate-limit, координация сервисов через Redis Pub/Sub. С реальными пользователями.</td>
      <td><a href="https://t.me/MedNapominalkaBot">@MedNapominalkaBot</a></td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/Ecoshop">Ecoshop</a></b></td>
      <td>Laravel 12 · React 19 · FSD · Meilisearch</td>
      <td>E-commerce платформа экотоваров: 12 моделей данных, RBAC из четырёх ролей, <code>lockForUpdate</code> против race condition при оформлении заказа, Feature-Sliced Design с автопроверкой Steiger в CI, PWA.</td>
      <td><a href="https://ecoshop.lavier.tech">ecoshop.lavier.tech</a></td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/portfolio-site">portfolio-site</a></b></td>
      <td>Next.js 16 · Go 1.25 · Postgres 16</td>
      <td>Двуязычный personal-brand сайт. JSONB-локализация в базе данных, push-based ISR revalidation, singleflight-кеш на Go перед Umami API, health-gate деплой с авто-rollback по <code>.last-good-sha</code>.</td>
      <td><a href="https://lavier.tech">lavier.tech</a></td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/TicketHub">TicketHub</a></b></td>
      <td>PHP 8.4 · MySQL 8 · REST API</td>
      <td>Тикет-система: REST API из ~45 эндпоинтов, defense-in-depth (SHA-256 хеширование токенов, защита от brute-force и SSRF, CIDR-allowlist), миграции с advisory locks. Оптимизация N+1 в JOIN на Kanban-доске: −99% запросов.</td>
      <td><a href="https://tickethub.lavier.tech">tickethub.lavier.tech</a></td>
    </tr>
  </tbody>
</table>

<h3>Machine learning и данные</h3>

<table>
  <thead>
    <tr>
      <th align="left">Проект</th>
      <th align="left">Стек</th>
      <th align="left">Что это</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b><a href="https://github.com/laviercasey/heart-disease-ml-benchmark">heart-disease-ml-benchmark</a></b></td>
      <td>Python · CatBoost · scikit-learn</td>
      <td>Многоцентровый ML-бенчмарк диагностики сердечно-сосудистых заболеваний (n = 1904 пациента, 8 алгоритмов, 6 баз данных). CatBoost ROC-AUC <b>0.948</b> с BCa-бутстреп доверительными интервалами и тестом DeLong. Код к опубликованной научной статье.</td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/metropt-predictive-maintenance">metropt-predictive-maintenance</a></b></td>
      <td>Python · GradientBoosting</td>
      <td>Раннее детектирование утечек воздуха в воздушном компрессоре поезда метро. ROC-AUC <b>0.9934</b>, F1 0.878 на 1.5 миллиона точек time-series (датасет MetroPT-3, UCI).</td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/GenreNeuro">GenreNeuro</a></b></td>
      <td>TensorFlow · Keras</td>
      <td>Нейросетевой классификатор жанров детских книг по текстовому описанию. Шесть жанров, точность <b>89%</b> (+58.9% над baseline).</td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/laviercasey/Children-book-dataset">Children-book-dataset</a></b> &nbsp;·&nbsp; <b><a href="https://github.com/laviercasey/Diafilm-Parts-Finder">Diafilm-Parts-Finder</a></b></td>
      <td>Python · BeautifulSoup · fuzzy matching</td>
      <td>Data-инструменты под библиотечный домен: парсер-датасет, на котором обучен GenreNeuro, и систематизация неструктурированной БД диафильмов (регулярные выражения + нечёткий поиск → Excel-отчёт по сериям и дубликатам).</td>
    </tr>
  </tbody>
</table>

<h2>Образование</h2>

<table>
  <tr>
    <td valign="top" width="18%"><b>2026</b></td>
    <td>Бакалавр, Московский университет имени С.Ю. Витте — <i>Прикладная информатика (искусственный интеллект и анализ данных)</i>. Курсовые ML-проекты в рамках специализации: обучение и оценка моделей на реальных данных.</td>
  </tr>
  <tr>
    <td valign="top"><b>2026</b></td>
    <td>karpov.courses — <i>Системный аналитик</i>. Сбор требований, моделирование бизнес-процессов (BPMN, UML), проектирование REST API, SQL, коммуникация со стейкхолдерами.</td>
  </tr>
  <tr>
    <td valign="top"><b>2021</b></td>
    <td>Московский государственный образовательный комплекс (МГОК) — <i>Сетевое и системное администрирование</i>. Трёхлетняя программа: TCP/IP и OSI, маршрутизация, администрирование Windows Server и Linux.</td>
  </tr>
</table>

<h2>Научные публикации</h2>

<ul>
  <li><b>«Сравнительный анализ алгоритмов машинного обучения для диагностики сердечно-сосудистых заболеваний на многоцентровой выборке»</b> — Лавьер К.М. Код и данные для воспроизведения результатов: <a href="https://github.com/laviercasey/heart-disease-ml-benchmark">heart-disease-ml-benchmark</a>. CatBoost ROC-AUC 0.948, n = 1904, 8 алгоритмов, 6 баз данных.</li>
</ul>

<h2>Production-опыт — РГДБ, четыре с лишним года</h2>

<ul>
  <li><b>SLA 99.9%</b> на стеке Prometheus + Grafana, прод-сервисы 24/7.</li>
  <li><b>MTTR −30%</b>, время диагностики −25% после реорганизации сетевой инфраструктуры с нуля.</li>
  <li><b>20+ production-скриптов</b> на Python и Bash: −60% ошибок рутины, экономия команде ~15 часов в неделю.</li>
  <li><b>Deploy-время с 2 часов до 15 минут</b> после внедрения CI/CD; простоев нет.</li>
  <li>Руковожу IT-командой из двух системных администраторов, менторю junior-специалиста.</li>
  <li>Технический аудит и документация систем управления музейными пространствами — организация перестала зависеть от вендора.</li>
  <li>База знаний из 50+ статей: время онбординга нового сотрудника сократилось с трёх недель до одной.</li>
</ul>

<h2>Фриланс</h2>

<p>
Параллельно с основной работой беру fullstack-engagement'ы по сарафанному радио — bug-fixes, выкатка фич и полные проекты с нуля для малого бизнеса, ИП и частных клиентов. Спектр задач: от разовых правок на несколько часов до проектов на один-три месяца.
</p>

<table>
  <tr>
    <td valign="top" width="22%"><b>Категории работ</b></td>
    <td>Поддержка и доработка существующих сайтов &nbsp;·&nbsp; реализация новых фич и интеграций (платёжные шлюзы, доставка, CRM, уведомления) &nbsp;·&nbsp; полные проекты с нуля &nbsp;·&nbsp; DevOps под ключ (VPS, SSL, Docker, CI/CD)</td>
  </tr>
  <tr>
    <td valign="top"><b>Стек</b></td>
    <td>Laravel &nbsp;·&nbsp; FastAPI &nbsp;·&nbsp; Next.js &nbsp;·&nbsp; React &nbsp;·&nbsp; PostgreSQL / MySQL &nbsp;·&nbsp; Docker &nbsp;·&nbsp; GitHub Actions &nbsp;·&nbsp; Caddy / Nginx &nbsp;·&nbsp; aiogram</td>
  </tr>
</table>

<p>
<sub>Большая часть кода живёт в приватных репозиториях клиентов под устными договорённостями; публичная витрина моего стека — open-source-проекты выше.</sub>
</p>

<h2>Контакты</h2>

<ul>
  <li>Портфолио — <a href="https://lavier.tech">lavier.tech</a></li>
  <li>Telegram — <a href="https://t.me/CaseyLav">@CaseyLav</a></li>
  <li>Email — <a href="mailto:laviercasey@gmail.com">laviercasey@gmail.com</a></li>
</ul>
