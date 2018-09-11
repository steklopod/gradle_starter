### Проект-стартер для Java 8 проекта. 

**5 ветвей** с разными настройками, в том числе конфигурация подключения к 2-ум БД (`MSSQL`, `MariaDB`).

В одном из бранчей находится пример работы с 2-мя БД: в качестве системы отправителя используется `MSSQL` server, а в 
качестве системы получателя приведен пример работы с БД типом `MariaDB`. Унифицировать работу с данными позволяет 
`Object Relationship Mapping (ORM)`, а точнее его реализация `JPA` от компании `Pivotal`, одной из ее дочерних компаний - `Spring`. 

В данном примере показана работа с фреймворком Spring Data.

+ Gradle

+ Postgres

+ Spring Boot 2.0

---

#### СБОРКА:
> A. Пароль и логин для БД проиписывается в папке ...\user-rebase\src\main\resources ,
в файле application.yml.

> Б. Необходимо, чтобы был установлен Gradle, в коммандной строке вводятся команды:

```groovy
1. `cd C:\Users\steklopod\...\user-app`

2. `gradle bootJar`

3. `cd build/libs`

4. `java -jar user-app-1.0.jar`
```

В папке `..\starter-post\src\test\resources` находятся **настройки Idea** `intellij_settings.jar` и используемые плагины.
[Инструкцйия по установке плагинов](https://github.com/shiraji/plugin-importer-exporter) `plugins.json`.

Чтобы узнать актуальные версии библиотек необходимо запустить таску gradle: `help` -> `dependencyUpdates`

#### Чтобы убить процесс на порту 8080 (Windows):
```
1. netstat -ano | findstr 8080
2. taskkill /pid @НОМЕР_ПОРТА@ /F
``` 
