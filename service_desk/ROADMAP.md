# ROADMAP — Service Desk «Хелпдеск»

Учебный роадмэп системного аналитика на сквозном проекте внутреннего портала ИТ-заявок.

## Паспорт

- **Формат:** 8–10 часов в неделю.
- **Срок:** ~25 недель, около 6 месяцев.
- **Объём:** 9 эпиков, 37 user stories.
- **Ритм:** 1 story = 1 карточка Kanban = 2–4 часа.
- **Подход:** итерации, артефакты уточняются по мере движения.
- **Фокус:** навыки системного анализа и портфолио, а не разработка кода.
- **Обновлено:** 2026-11-05.

## Цель

Пройти полный цикл системного анализа: от discovery и выявления требований до BPMN, ERD, API, NFR, UAT и защиты кейса в портфолио.

## Границы MVP

**Входит:**
- Создание и обработка заявок.
- Роли: сотрудник, агент поддержки, тимлид, администратор.
- Категории, приоритеты, назначение исполнителя.
- SLA, эскалация, статусы заявки.
- Комментарии и вложения.
- Email-уведомления через mock-сервис.
- Аудит действий.
- Базовые отчёты.

**Не входит:**
- Реальные SSO и email-интеграции.
- Платежи.
- Мобильные приложения.
- AI-классификация заявок.
- Мультитенантность.

## Легенда статусов

| Статус | Значение |
|---|---|
| `todo` | Не начато |
| `in progress` | В работе |
| `review` | На проверке |
| `done` | Артефакт готов и добавлен в портфолио |

## Definition of Done для story

1. Артефакт создан и лежит в структуре портфолио.
2. Проверен по чек-листу качества.
3. Связан с требованием, процессом или story.
4. Записан один вывод: что понял и что переделал бы.
5. Добавлен в индекс артефактов или портфолио.

## Карта эпиков

| ID | Эпик | Цель | Недели | Статус | Выход эпика |
|---|---|---|---:|---|---|
| E0 | Запуск и рамки | Понять проблему, пользователей и границы | 2 | `in progress` | Project brief, stakeholder map, glossary, context |
| E1 | Выявление требований | Собрать и проверить требования | 3 | `todo` | Interview guide, requirements register, change log |
| E2 | Процессы AS-IS/TO-BE | Разобрать текущий и целевой процесс | 3 | `todo` | 2 BPMN, pain points, RACI |
| E3 | User stories и use cases | Описать функциональность | 3 | `todo` | Story map, use cases, AC, traceability v1 |
| E4 | Данные | Спроектировать модель данных | 3 | `todo` | ERD, data dictionary, lifecycle |
| E5 | API и интеграции | Описать контракты и связи | 3 | `todo` | Integration map, OpenAPI, error catalog |
| E6 | NFR и безопасность | Сделать систему измеримой и безопасной | 3 | `todo` | NFR spec, RBAC, C4, ADR, security checklist |
| E7 | Тестирование и UAT | Проверить требования и приёмку | 3 | `todo` | Test scenarios, UAT, defect log, acceptance report |
| E8 | Портфолио и карьера | Упаковать опыт | 2 | `todo` | Portfolio case, demo, STAR, resume |

## Stories

### E0. Запуск и рамки

- [ ] `E0-S1` — Project brief — `in progress` — `stories/E0/E0-S1-project-brief.md`
- [ ] `E0-S2` — Stakeholder map — `todo` — `stories/E0/E0-S2-stakeholder-map.md`
- [ ] `E0-S3` — Glossary v1 — `todo` — `stories/E0/E0-S3-glossary.md`
- [ ] `E0-S4` — Context diagram + product canvas — `todo` — `stories/E0/E0-S4-context.md`
- [ ] `E0-S5` — Kanban + portfolio structure — `todo` — `stories/E0/E0-S5-kanban.md`

**Выход E0:** можно за 1 минуту объяснить, какую проблему решает «Хелпдеск» и что не входит в MVP.

### E1. Выявление и управление требованиями

- [ ] `E1-S1` — Interview guide + 3 интервью — `todo` — `stories/E1/E1-S1-interview-guide.md`
- [ ] `E1-S2` — Requirements register v1 — `todo` — `stories/E1/E1-S2-requirements-register.md`
- [ ] `E1-S3` — Requirements quality review — `todo` — `stories/E1/E1-S3-requirements-review.md`
- [ ] `E1-S4` — Change request + impact analysis — `todo` — `stories/E1/E1-S4-change-request.md`

**Выход E1:** реестр требований, который можно отдать на review, и один обработанный change request.

### E2. Процессы AS-IS и TO-BE

- [ ] `E2-S1` — BPMN AS-IS — `todo` — `stories/E2/E2-S1-bpmn-as-is.md`
- [ ] `E2-S2` — Pain points & root causes — `todo` — `stories/E2/E2-S2-pain-points.md`
- [ ] `E2-S3` — BPMN TO-BE — `todo` — `stories/E2/E2-S3-bpmn-to-be.md`
- [ ] `E2-S4` — Process review + RACI — `todo` — `stories/E2/E2-S4-process-review.md`

**Выход E2:** две BPMN-схемы и понятное объяснение, что меняется и зачем.

### E3. Функциональные требования, user stories и use cases

- [ ] `E3-S1` — User story map — `todo` — `stories/E3/E3-S1-user-story-map.md`
- [ ] `E3-S2` — Use case specs — `todo` — `stories/E3/E3-S2-use-cases.md`
- [ ] `E3-S3` — Acceptance criteria — `todo` — `stories/E3/E3-S3-acceptance-criteria.md`
- [ ] `E3-S4` — Traceability matrix v1 — `todo` — `stories/E3/E3-S4-traceability.md`

**Выход E3:** story map, use cases и матрица трассировки, по которым можно делать дизайн и тесты.

### E4. Данные и ERD

- [ ] `E4-S1` — Conceptual data model — `todo` — `stories/E4/E4-S1-conceptual-model.md`
- [ ] `E4-S2` — Data dictionary — `todo` — `stories/E4/E4-S2-data-dictionary.md`
- [ ] `E4-S3` — Logical ERD — `todo` — `stories/E4/E4-S3-erd.md`
- [ ] `E4-S4` — Data lifecycle + audit — `todo` — `stories/E4/E4-S4-data-lifecycle.md`

**Выход E4:** ERD и словарь данных, достаточные для проектирования API и БД.

### E5. API и интеграции

- [ ] `E5-S1` — Integration map — `todo` — `stories/E5/E5-S1-integration-map.md`
- [ ] `E5-S2` — OpenAPI v1 — `todo` — `stories/E5/E5-S2-openapi.md`
- [ ] `E5-S3` — Error catalog + idempotency — `todo` — `stories/E5/E5-S3-errors-idempotency.md`
- [ ] `E5-S4` — API review + ADR — `todo` — `stories/E5/E5-S4-api-review.md`

**Выход E5:** OpenAPI и карта интеграций, по которым можно писать код или моки.

### E6. NFR, безопасность и архитектура

- [ ] `E6-S1` — NFR specification — `todo` — `stories/E6/E6-S1-nfr.md`
- [ ] `E6-S2` — Permissions matrix (RBAC) — `todo` — `stories/E6/E6-S2-rbac.md`
- [ ] `E6-S3` — C4 + ADR-lite — `todo` — `stories/E6/E6-S3-c4-adr.md`
- [ ] `E6-S4` — Security checklist / threat model — `todo` — `stories/E6/E6-S4-security.md`

**Выход E6:** NFR, RBAC и ADR, которые можно защитить на review.

### E7. Тестирование, UAT и приёмка

- [ ] `E7-S1` — Test scenarios — `todo` — `stories/E7/E7-S1-test-scenarios.md`
- [ ] `E7-S2` — UAT checklist + protocol — `todo` — `stories/E7/E7-S2-uat.md`
- [ ] `E7-S3` — Defect log + regression set — `todo` — `stories/E7/E7-S3-defects.md`
- [ ] `E7-S4` — Traceability v2 + acceptance report — `todo` — `stories/E7/E7-S4-acceptance.md`

**Выход E7:** набор тестов, UAT и отчёт приёмки.

### E8. Портфолио, демо и карьера

- [ ] `E8-S1` — Portfolio case — `todo` — `stories/E8/E8-S1-portfolio-case.md`
- [ ] `E8-S2` — Demo script — `todo` — `stories/E8/E8-S2-demo.md`
- [ ] `E8-S3` — STAR stories — `todo` — `stories/E8/E8-S3-star.md`
- [ ] `E8-S4` — Resume + GitHub/Notion + mock interview — `todo` — `stories/E8/E8-S4-career-pack.md`

**Выход E8:** готовый портфолио-кейс и демо.

## Milestones

| Milestone | Что готово | Условие |
|---|---|---|
| M0. Discovery | Проблема, роли, словарь, контекст | E0 закрыт |
| M1. Требования и процессы | Требования и BPMN | E1 + E2 закрыты |
| M2. Решение описано | Stories, данные, API, NFR | E3–E6 закрыты |
| M3. Кейс готов | Тесты, UAT, портфолио | E7 + E8 закрыты |

## Зависимости

- E1 начинается после `E0-S1` и `E0-S2`.
- E2 начинается после `E1-S1`.
- E3 требует `E1-S2` и `E2-S3`.
- E4 требует `E3-S1`.
- E5 требует `E4-S3`.
- E6 требует `E3-S1` и `E5-S2`.
- E7 требует `E3-S4` и `E6-S1`.
- E8 требует завершения E7.

## Риски и допущения

| Риск | Как снизить |
|---|---|
| Расползание scope | Фиксировать out of scope в Project brief |
| Слишком долгие BPMN | Таймбокс 2 часа на схему |
| Нет обратной связи | Review в конце каждого эпика |
| Артефакты теряются | Индекс артефактов и единые ID |
| Пропущены требования | Traceability matrix и UAT |
| Перфекционизм | 1 story = 1 инкремент, версии 0.1, 0.2 |

## Текущий фокус

1. `E0-S1` — Project brief.
2. `E0-S2` — Stakeholder map.
3. `E0-S3` — Glossary v1.

## Прогресс

- Всего stories: **37**.
- Done: **0**.
- In progress: **1**.
- Todo: **36**.

## Правила ведения роадмэпа

- Статус story меняется в одном месте: в этой карте и в файле story.
- Полные описания, AC и заметки живут в `stories/`, а не здесь.
- Артефакты живут в `artifacts/` и индексируются в `docs/artifact-index.md`.
- ID не меняются после создания.
- В конце эпика обновляются milestone, прогресс и текущий фокус.

## Ссылки

- [README](README.md)
- [Индекс артефактов](docs/artifact-index.md) — создать в E0-S5.
- [Матрица трассировки](docs/traceability.md) — создать в E3-S4.
- [Портфолио-кейс](portfolio/case.md) — создать в E8-S1.
