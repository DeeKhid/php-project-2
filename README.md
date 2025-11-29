### Hexlet tests and linter status:
[![Actions Status](https://github.com/fzxcvbn/php-project-48/actions/workflows/hexlet-check.yml/badge.svg)](https://github.com/fzxcvbn/php-project-48/actions)
[![Actions Status](https://github.com/fzxcvbn/php-project-48/actions/workflows/check.yml/badge.svg)](https://github.com/fzxcvbn/php-project-48/actions)
[![Maintainability](https://api.codeclimate.com/v1/badges/97a85b243d3115e26757/maintainability)](https://codeclimate.com/github/fzxcvbn/php-project-48/maintainability)
[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fzxcvbn_php-project-48&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fzxcvbn_php-project-48)
# Вычислитель отличий
Вычислитель отличий – программа, определяющая разницу между двумя структурами данных. Это популярная задача, для решения которой существует множество онлайн-сервисов, например: http://www.jsondiff.com/. Подобный механизм используется при выводе тестов или при автоматическом отслеживании изменении в конфигурационных файлах.

### Возможности утилиты:
- Поддержка разных входных форматов: yaml и json
- Генерация отчета в виде plain text, stylish и json

### Пример использования:
```
gendiff --format plain path/to/file.yml another/path/file.json

Property 'common.follow' was added with value: false
Property 'group1.baz' was updated. From 'bas' to 'bars'
Property 'group2' was removed

# формат stylish
gendiff filepath1.json filepath2.json

{
  + follow: false
    setting1: Value 1
  - setting2: 200
  - setting3: true
  + setting3: {
        key: value
    }
  + setting4: blah blah
  + setting5: {
        key5: value5
    }
}
```

[![asciicast](https://asciinema.org/connect/ae644b7a-5871-455d-98a8-15726ccf950a.svg)](https://asciinema.org/connect/ae644b7a-5871-455d-98a8-15726ccf950a)

