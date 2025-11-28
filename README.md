## Имя: Дорджиев Виктор
## Группа: ЭФМО-02-25
# Проект pz7-redis

Задачи проекта
1)	Освоить базовые операции работы с Redis из Go-приложения.
2)	Научиться использовать команды SET, GET, задавать время жизни ключей (TTL).
3)	Реализовать кэширование данных для ускорения работы API.
4)	Понять, в каких случаях кэш помогает снизить нагрузку на базу данных.

---

## Установка и запуск

(Необходимы предустановленные Go и Git)

Клонировать репозиторий:

```
git clone https://github.com/Unpatches/pz7-redis
cd pz7-redis
```

Команда запуска сервера:

```
go run ./cmd/server
```


------

## Структура проекта

```plaintext
pz7-redis/                     
├── cmd/                  
│   └── server/             
│       └── main.go       
├── internal/              
│   └── cache/               
│   │   └── cache.go           
├── go.mod                
└── go.sum       
```

## Отчёт о проделанной работе
установка значения POST
```
http://217.119.129.232:8080/set?key=test&value=hello
```

<img width="475" height="433" alt="image" src="https://github.com/user-attachments/assets/cb096837-6639-4c96-b605-5b85dd2da72c" />

получение значения GET
```
http://217.119.129.232:8080/get?key=test
```

<img width="423" height="400" alt="image" src="https://github.com/user-attachments/assets/b2725afd-72a8-4bdb-b742-eede225cfd7c" />

проверка TTL GET
```
http://217.119.129.232:8080/ttl?key=test
```

<img width="384" height="407" alt="image" src="https://github.com/user-attachments/assets/07301e96-df2e-40f3-be2a-0d399ee6d0e2" />

------


