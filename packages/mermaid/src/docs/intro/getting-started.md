graph LR
    A[Пользователь (Telegram)] --> B(Telegram Bot API);
    B --> C{Сервер (Heroku)};
    C --> D[Python (python-telegram-bot)];
    D --> E[SQLAlchemy ORM];
    E --> F((PostgreSQL DB));
    C --> G{Edamam API (Опционально)};

    subgraph "Инструменты разработки"
        H[IDE (PyCharm/VS Code)]
        I[Git/GitHub (VCS)]
        J[pip (Package Manager)]
        K[pytest/unittest (Testing)]
    end

    subgraph "Безопасность"
        L[HTTPS (Шифрование)]
        M[bcrypt/Argon2 (Хеширование паролей)]
        N[Защита от SQL Injection]
        O[Защита от XSS]
        P[Регулярные обновления]
        Q[Статический анализ кода (Bandit)]
    end

    style A fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#ccf,stroke:#333,stroke-width:2px
    style C fill:#fcc,stroke:#333,stroke-width:2px
    style D fill:#fcc,stroke:#333,stroke-width:2px
    style E fill:#ccf,stroke:#333,stroke-width:2px
    style F fill:#ccf,stroke:#333,stroke-width:2px
    style G fill:#fcc,stroke:#333,stroke-width:2px
    style H fill:#fff,stroke:#333,stroke-width:1px
    style I fill:#fff,stroke:#333,stroke-width:1px
    style J fill:#fff,stroke:#333,stroke-width:1px
    style K fill:#fff,stroke:#333,stroke-width:1px
    style L fill:#fff,stroke:#333,stroke-width:1px
    style M fill:#fff,stroke:#333,stroke-width:1px
    style N fill:#fff,stroke:#333,stroke-width:1px
    style O fill:#fff,stroke:#333,stroke-width:1px
    style P fill:#fff,stroke:#333,stroke-width:1px
    style Q fill:#fff,stroke:#333,stroke-width:1px

    linkStyle 0 stroke:#333,stroke-width:2px;
    linkStyle 1 stroke:#333,stroke-width:2px;
    linkStyle 2 stroke:#333,stroke-width:2px;
    linkStyle 3 stroke:#333,stroke-width:2px;
    linkStyle 4 stroke:#333,stroke-width:2px;
    linkStyle 5 stroke:#333,stroke-width:2px;
    linkStyle 6 stroke:#333,stroke-width:1px,stroke-dasharray:5 5; // Edamam - опциональный

    click A "https://telegram.org/" "Открыть Telegram"
    click B "https://core.telegram.org/bots/api" "Открыть Telegram Bot API"
    click C "https://www.heroku.com/" "Открыть Heroku"
    click D "https://www.python.org/" "Открыть Python"
    click E "https://www.sqlalchemy.org/" "Открыть SQLAlchemy"
    click F "https://www.postgresql.org/" "Открыть PostgreSQL"
    click G "https://www.edamam.com/" "Открыть Edamam API"
