# go-foundation

Учебный репозиторий фундамента Go в рамках 100-дневной подготовки
(Go/MLOps + английский). Код пишется руками, без автогенерации.

## Структура (Фаза 1 — Фундамент, дни 5–35)

Каждая неделя — отдельная тема. Папки появляются по мере прохождения:

| Неделя | Папка | Тема |
|--------|-------|------|
| A | `language/` | structs, методы, интерфейсы, ошибки, slices/maps, net/http |
| B | `concurrency/` | goroutines, каналы, select, context, worker pool |
| C | `testing-db/` | table-driven тесты, httptest, Postgres, repository |
| D | `production/` | logging, config, graceful shutdown, Docker, compose |

Итог фазы — рабочий `net/http` JSON-сервис с БД, тестами, concurrency,
упакованный в Docker.

## Запуск

```bash
go run ./<папка>
go test ./...
go vet ./...
```
