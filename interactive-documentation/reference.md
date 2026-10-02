
## Основные эндпоинты API

| Метод | Эндпоинт | Назначение |
| POST | `/api/auth/register` | Регистрация гостя |
| POST | `/api/auth/login` | Авторизация |
| GET | `/api/rooms` | Список номеров |
| POST | `/api/bookings` | Создание бронирования |
| GET | `/api/admin/bookings` | Все бронирования (админ) |

## Параметры бронирования

| Поле | Тип | Обязательное | Описание |
| roomId | integer | Да | ID комнаты |
| checkIn | string | Да | Дата заезда (YYYY-MM-DD) |
| checkOut | string | Да | Дата выезда (YYYY-MM-DD) |

## Пример запроса на создание бронирования

```bash
curl -X POST http://localhost:8080/api/bookings \
  -H "Authorization: Bearer <token>" \
  -H "Content-Type: application/json" \
  -d '{"roomId": 101, "checkIn": "2026-10-01", "checkOut": "2026-10-05"}'
