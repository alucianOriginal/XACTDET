X-ANTI-CORRUPTION-TEXT-DETECTOR
This is a Tool to detect Corruption in Text over Noise Analysis


├── main.py              # Der Startpunkt (Steuerung)
├── logic/
│   ├── consistency.py   # Säule 1: Logikprüfung
│   ├── noise_floor.py   # Säule 2: Stilprofil-Analyse
│   └── cognitive.py     # Säule 3: Distanzsprache-Check
├── data/
│   └── patterns.json    # "Wörterbuch" für verdächtige Begriffe (Juristendeutsch)
└── reports/             # Hier landen die Ergebnisse
