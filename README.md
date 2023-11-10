```mermaid
sequenceDiagram
    participant S as Студент
    participant E as Електронний каталог
    participant R as Реєстраційна система
    participant C as Курс

    S->>E: Запит доступних місць на курсі
    E-->>S: Відображення кількості місць
    S->>R: Надсилання запиту на реєстрацію
    R->>C: Перевірка наявності місць
    C-->>R: Підтвердження наявності місця
    R-->>S: Підтвердження реєстрації на курс

