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
http://193.233.171.146:8080/set?key=test&value=hello
```
получение значения GET
```
http://193.233.171.146:8080/get?key=test
```
проверка TTL GET
```
http://193.233.171.146:8080/ttl?key=test
```
<img width="442" height="399" alt="image" src="https://github.com/user-attachments/assets/8abedb59-dae4-4480-baa6-eb365e84bd32" />
<img width="378" height="397" alt="image" src="https://github.com/user-attachments/assets/48771c93-426b-4b65-9f95-a1232274b8ac" />
<img width="369" height="407" alt="image" src="https://github.com/user-attachments/assets/c9a9816c-26c9-40be-967c-9df8b1ff7151" />


