# go_url_shortener

Учебный проект сокращателя ссылок на Go.

Запускать из корня репозитория — папки, где находится `go.mod`:

```bash
CONFIG_PATH=./config/local.yaml go run ./cmd/url-shortener
```

`CONFIG_PATH` задаёт путь к YAML-конфигу. Относительные пути, включая
`storage_path` внутри конфига, считаются от рабочей папки процесса.
SQLite создаёт файл `storage/storage.db`; папка `storage` хранится в Git
через пустой файл `.gitkeep`, а файлы базы игнорируются.

Проверка компиляции пакетов:

```bash
go test ./...
```
