erDiagram
    STUDIOS ||--o{ GAMES : develops
    GAMES ||--o{ PLAY_SESSIONS : has_sessions

    STUDIOS {
        string studio_name PK
        string country
        int founded_year
    }

    GAMES {
        string game_title PK
        string studio_name FK
        string platform
        string genres
        string status
        date added_date
        float planned_hours
        float played_hours
        string progress
        string complete_action
    }

    PLAY_SESSIONS {
        string session_title PK
        string game_title FK
        date session_date
        float duration_hours
        string impression
    }
