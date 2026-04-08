# Converted Proto Repository

Репозиторий для сгенерированных Go файлов из .proto.

## Что уже готово

- Workflow: .github/workflows/generate.yml
- Модуль Go: go.mod

## Что заменить под себя

1. В go.mod:
- github.com/your-user/converted-protos -> твой github user и имя этого репозитория

2. В .github/workflows/generate.yml:
- branches: main или master
- PROTO_REPO: owner/protos-repo
- GIT_USER_NAME, GIT_USER_EMAIL

3. В proto файлах (в proto-репозитории) обязательно обнови go_package на этот generator repo.

## Как запускать генерацию

- Открой Actions
- Выбери workflow Generate Protobuf Go Files
- Нажми Run workflow

## Релиз (тег)

Сделай вручную через Releases:

- v1.0.0 для первого релиза
- v1.0.1, v1.0.2 для мелких изменений
- v1.1.0 и выше для major изменений

## Подключение в других проектах

go get github.com/ayatyeah/converted-protos@v1.0.0
