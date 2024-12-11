# Instagram Bot Manager

Sistem automat de gestionare conturi Instagram cu autentificare prin cookie-uri și integrare Gemini.

## Funcționalități

- Autentificare prin cookie-uri
- Integrare cu Gemini pentru răspunsuri inteligente
- Dashboard de monitorizare
- Sistem avansat de logging
- Rate limiting și gestionare erori
- Metrici și statistici

## Instalare

1. Clonează repository-ul:
```bash
git clone https://github.com/fggmfsii/instagram-bot-manager.git
cd instagram-bot-manager
```

2. Instalează dependințele:
```bash
pip install -r requirements.txt
```

3. Configurează setările în `config/settings.py`

4. Adaugă cookie-urile în fișierul `instagram_cookies.json`

## Utilizare

1. Pornește serverul:
```bash
python run.py
```

2. Accesează dashboard-ul la:
```
http://localhost:5000/dashboard
```

## Structura proiectului

```
instagram-bot-manager/
├── src/
│   ├── config/
│   │   └── settings.py
│   ├── dashboard/
│   │   ├── templates/
│   │   └── routes.py
│   ├── models/
│   │   ├── conversation.py
│   │   └── interaction.py
│   ├── services/
│   │   ├── instagram_service.py
│   │   ├── gemini_service.py
│   │   └── feed_service.py
│   └── utils/
│       ├── cookie_manager.py
│       ├── rate_limiter.py
│       └── error_handler.py
├── logs/
├── data/
└── requirements.txt
```