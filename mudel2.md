```mermaid
sequenceDiagram
    participant Студент
    participant CourseCatalog
    participant Course
    participant RegistrationSystem

    Student->>CourseCatalog: запрос информации о курсах
    CourseCatalog-->>Student: информация о курсах
    Student->>RegistrationSystem: запрос на регистрацию
    RegistrationSystem->>Course: проверка доступности мест
    Course-->>RegistrationSystem: информация о доступности
    RegistrationSystem-->>Student: подтверждение/отказ регистрации
