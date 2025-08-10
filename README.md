# Vector Role

Ansible роль для установки и настройки Vector (лог-агента).

## Переменные

| Переменная | По умолчанию | Описание |
|------------|--------------|----------|
| `vector_version` | "0.34.0" | Версия Vector |
| `vector_user` | "vector" | Пользователь для запуска Vector |
| `vector_config_dir` | "/etc/vector" | Директория для конфигурации |
| `clickhouse_host` | "localhost" | Хост ClickHouse |
| `clickhouse_db` | "default" | База данных ClickHouse |
| `clickhouse_table` | "logs" | Таблица для логов |

## Использование
```yaml
- hosts: vector_hosts
  roles:
    - vector-role
