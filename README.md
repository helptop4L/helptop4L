sequenceDiagram
    participant Student as "Студент"
    participant Catalog as "Електронний каталог"
    participant RegSystem as "Реєстраційна система"
    participant Course as "Курс"

    Student->>+Catalog: Запит на перевірку доступних місць
    Catalog-->>-Student: Відображення кількості доступних місць

    Student->>+RegSystem: Подача заявки на реєстрацію
    RegSystem->>+Course: Перевірка доступності місць
    Course-->>-RegSystem: Підтвердження наявності місць
    RegSystem-->>-Student: Підтвердження реєстрації на курс
