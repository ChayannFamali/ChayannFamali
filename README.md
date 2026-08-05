<h1 align="center">Дмитрий Веселов</h1>

<p align="center">
  <b>Data Engineer · ML/LLM Engineer · Computer Vision Researcher</b><br>
  <i>Высоконагруженные ETL/ELT-пайплайны · LLM fine-tuning и RAG · надёжность нейросетей</i>
</p>

<p align="center">
  <a href="https://t.me/ChayannDMWork"><img src="https://img.shields.io/badge/-Telegram-0088cc?style=flat&logo=telegram&logoColor=white"></a>
  <a href="mailto:dima.veselow2011@yandex.ru"><img src="https://img.shields.io/badge/-Email-D14836?style=flat&logo=maildotru&logoColor=white"></a>
  <a href="https://github.com/ChayannFamali"><img src="https://img.shields.io/badge/-GitHub-181717?style=flat&logo=github"></a>
  <a href="https://huggingface.co/ChayannFamali"><img src="https://img.shields.io/badge/-HuggingFace-FFD21E?style=flat&logo=huggingface&logoColor=black"></a>
  <a href="https://www.kaggle.com/dmitriyveselov"><img src="https://img.shields.io/badge/-Kaggle-20BEFF?style=flat&logo=kaggle&logoColor=white"></a>
  <a href="https://elibrary.ru/author_items.asp?authorid=1094423"><img src="https://img.shields.io/badge/-eLibrary-1f6feb?style=flat&logo=googlescholar&logoColor=white"></a>
</p>

---

## 🧑‍💻 О себе

> Data Engineer с фокусом на высоконагруженные ETL/ELT-пайплайны и исследователь в области Computer Vision, LLM и надёжности нейронных сетей.

- 📍 **Локация:** Москва, Россия · удалённая работа и гибрид
- 💼 **Сейчас:** Старший разработчик @ Гринатом · Научный сотрудник лаборатории компьютерного зрения и робототехники @ Финуниверситет
- ⚙️ **Опыт:** 5+ лет в Data Engineering и ETL/ELT · 3+ года в ML/DL и Computer Vision
- 🎓 **Образование:** магистр прикладной математики и информатики (Финуниверситет, 2022) · соискатель PhD по направлению 1.2.1 «Искусственный интеллект и машинное обучение»
- 🔬 **Наука:** 14 публикаций (Scopus / IEEE Xplore / ВАК / РИНЦ), доклады на 5+ конференциях
- ✍️ **Диссертация:** *«Численные методы оценивания и контроля локальной константы Липшица нейросетевых моделей и их применение для анализа и повышения устойчивости к состязательным возмущениям»*
- 🌐 **Языки:** русский — native · английский — B2 (IELTS, 2020)

---

## 🛠️ Технический стек

**Языки:** Python · Java · Go · C++ · Scala · SQL · TypeScript

| Категория | Технологии |
|---|---|
| **Data Engineering / ETL** | Apache NiFi · Airflow · Kafka · Druid · Dremio · Liquibase · SAP BW |
| **Базы данных** | PostgreSQL · ClickHouse · Greenplum · ArenaDB · Elasticsearch · MongoDB · Neo4j · SQLite |
| **LLM / NLP** | Hugging Face Transformers · sentence-transformers · LangChain · LangGraph · LlamaIndex · vLLM · Ollama · LM Studio |
| **LLM Fine-tuning** | QLoRA / LoRA (PEFT) · NF4-квантизация · bitsandbytes · Qwen2.5-Coder |
| **Retrieval / RAG** | BM25 (собственная реализация) · dense retrieval (bge-m3) · hybrid search · RRF · re-ranking · HyDE · ChromaDB · FAISS · Qdrant · pgvector · hnswlib |
| **ML / DL / CV** | PyTorch · TensorFlow · Keras · scikit-learn · OpenCV |
| **Backend** | FastAPI · Django · Flask · Spring Boot · Go (net, gRPC, TCP-proxy) |
| **Systems / Go** | PostgreSQL Wire Protocol · pgproto3 · pg_query_go (SQL AST) · Cobra CLI · Chi router |
| **Frontend** | React 19 · TypeScript · Vite · TanStack Query · htmx + SSE · Streamlit |
| **Observability / Security** | Prometheus · Grafana · OIDC · RBAC · audit trail (hash-chain) |
| **DevOps** | Docker · Docker Compose · Kubernetes · CI/CD · Git · Linux |
| **BI / Analytics** | Tableau · SAS |
| **Trading / Quant** | T-Invest API · портфельная теория · risk-parity · VaR / CVaR / Sharpe · backtesting |

---

## 🏆 Ключевые достижения

### ⚙️ Data Engineering и платформа

- 🚀 **Спроектировал и вывел в прод ETL-платформу** на стеке Apache NiFi + Java + ArenaDB взамен legacy-конвейера — обработка **>1 млн записей в сутки**. Реализовал семантику **at-least-once с идемпотентной записью** (дедупликация по бизнес-ключу), что исключило дубли в целевом хранилище.
- ⚡ **Ускорил загрузку данных в ~7×** (батч 200 тыс. записей: с ~200–240 до ~30 сек) за счёт батчинга, параллелизма и оптимизации схемы хранения.
- 🔧 **Ускорил этап трансформации в ~5×** (с ~5 до ~1 мин): профилировал пайплайн, переписал неоптимальные запросы, добавил индексы и перенёс часть логики в NiFi на Groovy.
- 🗄️ **Снизил нагрузку на БД на ~20%** (CPU и время выполнения тяжёлых запросов) через рефакторинг структур данных, партиционирование и перенос аналитических нагрузок на колоночное хранилище (ClickHouse).
- 🔁 **Перевёл часть пакетных пайплайнов на near-real-time стриминг** (Kafka + Airflow), сократив задержку доставки данных аналитикам с нескольких часов до единиц минут.
- 🧩 **Разработал 4 интеграционных REST API на Spring Boot** поверх потоков NiFi — единый контракт (OpenAPI + аутентификация) вместо точечных интеграций внутренних команд.
- 📉 **Внедрил Data Quality-проверки и мониторинг пайплайнов** (валидация на входе, метрики, алерты), снизив число инцидентов с «битыми» данными на проде с ~20 до ~13 в месяц (**~35%**).
- 🏗️ **Спроектировал схемы загрузки и хранения DWH**, обслуживающего 6 аналитических витрин и команд; ускорил ключевые отчёты на **40%**; настроил миграции схем через Liquibase, исключив ручные правки на релизах.
- 🧰 **Стандартизировал инфраструктуру через Docker и CI/CD**, сократив время развёртывания нового пайплайна с нескольких дней до нескольких часов.

### 🤖 LLM / AI Engineering

- 🧠 **QLoRA fine-tuning Qwen2.5-Coder (7B и 14B)** под ABAP/SQL: корпус **812 тыс. примеров кода** (14 языков, 13 источников), обучение на стратифицированных выборках **100 тыс.** (7B, 12,9% ABAP) и **50 тыс.** (14B).
- 🔍 **Hybrid RAG поверх дообученной модели:** dense retrieval (bge-m3) + BM25 + Reciprocal Rank Fusion, few-shot-инъекция примеров на инференсе. Корпус — 20 тыс. документов → 59 тыс. structure-aware чанков в ChromaDB.
- 📈 **Результат (fine-tuning + RAG vs baseline):** ABAP chrF **0,325 → 0,531 (+63%)**, SQL exact match **0,04 → 0,38 (9,5×)**.
- 🎯 **Устранил Python-switching** (модель генерирует Python вместо ABAP): 17,8% → **0%** на валидации — чисто inference-time фиксом через retrieval, **без переобучения**.
- 🧪 **Честный eval:** 325 held-out промптов, отсутствие утечек подтверждено сверкой content-hash; отдельно зафиксированы trade-off'ы (просадка syntax_valid у 14B+RAG, регресс Java при ABAP-boosted обучении).
- 💻 **Всё обучение — на двух consumer-GPU** (RTX 4000 Ada 20 ГБ + RTX 5070 12 ГБ) за счёт NF4 + double quantization, без кластера.
- 🤗 **Модели опубликованы:** [huggingface.co/ChayannFamali](https://huggingface.co/ChayannFamali)

### 🔬 Наука и исследования

- 📚 **14 научных публикаций** в рецензируемых изданиях (Scopus / IEEE Xplore / ВАК / РИНЦ).
- 🏅 Статья по **генеративным моделям для поиска лекарственных соединений** — победитель Международного салона образования.
- 🧠 Алгоритмы CV для **медицинской диагностики**: детекция внутричерепных кровоизлияний и переломов шейного отдела позвоночника, семантическая сегментация КТ/МРТ.
- 🛡️ Текущее исследование — **устойчивость нейросетей к состязательным атакам** через оценивание и контроль локальной константы Липшица.

---

## 📄 Научные публикации

| Год | Публикация | Издание / Сборник |
|---|---|---|
| 2026 | Ансамблевые методы машинного обучения для прогностической диагностики сердечно-сосудистых заболеваний: сравнительный анализ на многоцентровой выборке | Моделирование, оптимизация и информационные технологии |
| 2026 | Рентгеномная классификация опухолей головного мозга методами искусственного интеллекта | РЛНС, XXXII Междунар. науч.-техн. конференция |
| 2025 | Оптимизация процесса обучения в интеллектуальной системе распознавания документов | Автоматизация процессов управления, №3(81) |
| 2025 | Интеллектуальная обработка финансовых документов с применением технологий больших языковых моделей | Экономика строительства, №8 |
| 2025 | Распознавание документов в различных условиях с помощью методов машинного обучения | Нелинейный мир, Т.23 №3 |
| 2025 | Обзор математических моделей и алгоритмов нейросетевого распознавания зон интереса на основе анализа радиологической информации | Современная наука, №3 |
| 2024 | [**Detection of Intracranial Hemorrhage by AI and Deep Learning** *(Scopus)*](https://ieeexplore.ieee.org/document/10582393) | IEEE ITNT 2024 |
| 2024 | Обнаружение внутричерепного кровоизлияния методами искусственного интеллекта † | ИТНТ-2024, Самара |
| 2024 | Обнаружение переломов шейного отдела позвоночника методами искусственного интеллекта | Нейрокомпьютеры, Т.26 №6 |
| 2024 | Сегментация медицинских изображений с использованием методов компьютерного зрения | РЛНС, Воронеж |
| 2024 | Искусственные нейронные сети в анализе медицинских снимков | Сб. науч. трудов, Ульяновск |
| 2023 | Обнаружение лиц с помощью гибридных детекторов | ММРО-21, Москва |
| 2023 | Математические алгоритмы предупреждения аварийных ситуаций на основе данных видеокамеры | РЛНС, Воронеж |
| 2022 | Применение генеративных моделей для предсказания лекарственных молекулярных соединений | Современные наукоёмкие технологии, №3 |

<sub>† RU-версия доклада, англоязычная версия индексирована в Scopus / IEEE Xplore.</sub>

🔗 [Полный список публикаций на eLibrary](https://elibrary.ru/author_items.asp?authorid=1094423)

---

## 🚀 Проекты

### 🤖 AI / LLM Engineering

- **[Qwen-Coder ABAP RAG](https://github.com/ChayannFamali/qwen-coder-abap-rag)** — QLoRA fine-tuning `Qwen2.5-Coder 7B/14B` + Hybrid RAG (dense + BM25 + RRF) для генерации ABAP/SQL.
  Корпус 812k примеров → обучение на 100k/50k; ABAP chrF +63%, SQL exact match 9,5×, Python-switching 17,8% → 0%.
  Zero-leakage eval на 325 промптах, воспроизводимый пайплайн, модели на HuggingFace.

- **SciAssist** — локальный офлайн RAG-ассистент для научной работы: `Zotero · LM Studio · ChromaDB · Obsidian`.
  Hybrid retrieval + re-ranking + HyDE, полностью на своём железе без внешних API.

- **HybridSearch** — поисковый стек для RAG на CPU без GPU: собственная реализация BM25, dense retrieval, RRF-гибрид.
  Eval-фреймворк (nDCG / MRR / recall) на датасетах BEIR.

### 🧱 Systems / Go

- **ReconCore** — декларативный движок сверки данных на `Go`: каскад exact → tolerance → fuzzy → ML,
  audit trail с hash-chain, React-workbench. **1 млн записей за 21 сек.**

- **QueryGuard** — TCP-proxy перед PostgreSQL: разбор SQL через AST (`pg_query_go`), реализация PostgreSQL Wire Protocol,
  детекция N+1 / `SELECT *` / отсутствия `LIMIT`, policy engine, дашборд на `htmx + SSE` без фронтенд-фреймворка.

### ⚙️ Data Engineering

- **ETL-платформа** — высоконагруженная система обработки данных на `Apache NiFi · Java · ArenaDB`.
  >1 млн записей в сутки, at-least-once с идемпотентной записью; загрузка ускорена ~7×, трансформация ~5×.

- **Data Access API** — сервис на `Spring Boot` как единая точка доступа к данным в потоках NiFi.
  REST-запросы от внутренних команд → маршрутизация в обработку (Kafka / NiFi `ListenHTTP`) → результат.
  Единый контракт OpenAPI с аутентификацией вместо прямых интеграций.

- **Streaming Data Pipeline** — near-real-time доставка данных на `Kafka · Airflow`.
  Перевод пакетных пайплайнов на стриминг: задержка с часов до минут.

- **Data Quality & Monitoring** — слой контроля качества пайплайнов: валидация на входе, метрики, алерты.
  Снижение инцидентов с «битыми» данными на ~35%.

### 📈 Quant / Trading

- **T-Invest Portfolio Rebalancer** — автоматический ребалансер портфеля (акции / облигации / металлы / кэш) на MOEX
  через `T-Invest API`. Risk-parity, circuit breaker, бэктест, money-safe вычисления на `Decimal`.

- **[Reinforcement Learning in Trading](https://github.com/ChayannFamali/Reinforcement-learning-in-Trading)** — RL-алгоритмы для финансовых рынков.

### 👁️ Machine Learning / Computer Vision

- **[Drug Discovery ML](https://github.com/ChayannFamali/Application-of-generative-models-for-prediction-of-drug-molecular-compounds)** — генеративные модели для предсказания лекарственных молекулярных соединений.
- **[Circadian Rhythm Analysis](https://brightmagazine.ru/искусственный-интеллект-растени/)** — анализ биологических ритмов методами глубокого обучения.
- **Гибридная детекция лиц** — комбинация классических и нейросетевых детекторов.
- **Сегментация медицинских изображений** — диагностика патологий на КТ/МРТ.
- **Видеоаналитика** — предупреждение аварийных ситуаций в задачах промышленной безопасности.

---

## 🤗 Модели на HuggingFace

| Модель | Описание |
|---|---|
| [qwen14b-abap-sql-lora](https://huggingface.co/ChayannFamali/qwen14b-abap-sql-lora) | QLoRA-адаптер для `Qwen2.5-Coder-14B-Instruct`, ABAP/SQL, 50k сэмплов |
| [qwen7b-abap-sql-lora](https://huggingface.co/ChayannFamali/qwen7b-abap-sql-lora) | QLoRA-адаптер для `Qwen2.5-Coder-7B-Instruct`, ABAP/SQL, 100k сэмплов (12,9% ABAP) |

---

## 💼 Опыт работы

| Период | Роль | Компания |
|---|---|---|
| 07.2024 — н.в. | Старший разработчик | Гринатом |
| 02.2023 — н.в. | Научный сотрудник, лаборатория компьютерного зрения и робототехники | Финансовый университет |
| 09.2021 — 07.2024 | Data Engineer | Goodt |
| 08.2021 — 09.2021 | Стажёр-аналитик, департамент Data & Analytics | Citibank |

---

## 🎓 Образование

- **Соискатель PhD** — 1.2.1 Искусственный интеллект и машинное обучение · Финуниверситет (2026 — н.в.)
- **Магистратура** — Прикладная математика и информатика · Финуниверситет (2020 — 2022)
- **Бакалавриат** — Прикладная математика и информатика · Финуниверситет (2016 — 2020)

---

## 📈 Профессиональное развитие

- 🎓 Deep Learning School — МФТИ (2021 — 2022)
- 🤖 Deep Learning Engineer — Karpov.Courses (2025)
- 👁️ Deep Learning Engineer. Computer Vision — Karpov.Courses (2025)
- 🧱 System Design — Karpov.Courses (2025)
- 🐳 Администрирование Docker (2024)
- 📜 [Дополнительные сертификаты](https://stepik.org/users/23936910/certificates)

---

## 📫 Контакты

Открыт для интересных проектов, сотрудничества и научной работы.

- **Telegram:** [@ChayannDMWork](https://t.me/ChayannDMWork)
- **Email:** [dima.veselow2011@yandex.ru](mailto:dima.veselow2011@yandex.ru)
- **HuggingFace:** [ChayannFamali](https://huggingface.co/ChayannFamali)
- **Kaggle:** [dmitriyveselov](https://www.kaggle.com/dmitriyveselov)
- **eLibrary:** [authorid 1094423](https://elibrary.ru/author_items.asp?authorid=1094423)

---

## 📊 GitHub Statistics

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=ChayannFamali&theme=tokyonight" height="170">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=ChayannFamali&theme=tokyonight" height="170">
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=ChayannFamali&theme=tokyonight" height="170">
</p>
