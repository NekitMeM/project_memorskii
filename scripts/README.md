В данной папке размещаем скриптовые файлы *.js
# Динамические и интерактивные элементы  

## **1. Формы**  
- **Форма записи** (`.enrollment-form`):  
  - Отправка данных в Telegram.  
  - Валидация полей.  
  Код блока-схемы для mermaid:
  flowchart TD
    A[Пользователь заполняет форму] --> B{Поля валидны?}
    B -->|Да| C[Показать загрузку]
    B -->|Нет| D[Показать ошибку]
    C --> E[Отправить данные в Telegram]
    E --> F{Успешно?}
    F -->|Да| G[Показать 'Успешно отправлено!']
    F -->|Нет| H[Показать 'Ошибка отправки']
    G --> I[Сбросить форму]
    H --> I

## **2. Модальное окно**  
- **Кнопки "Записаться"**: Открывают модальное окно (`#enrollmentModal`).  
- **Навигация по шагам**: Переключение между выбором преподавателя и временем.  

## **3. Адаптивность**  
- Изменение сетки преподавателей и фич при `width < 768px`.  
