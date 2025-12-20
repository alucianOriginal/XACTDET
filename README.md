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


Projekt-Konzept: XACTDET (Kohärenzdetektor)
1. Der Kernzweck

XACTDET ist kein „Lügen-Detektor“ oder Moralwerkzeug, sondern ein Kohärenzdetektor. Das Ziel ist es, sprachliche Verantwortungsflucht und asymmetrische Machtverhältnisse in Texten (wie Reports, Kündigungen oder Behördenschreiben) sichtbar zu machen. Es misst nicht die subjektive Schuld, sondern die objektive Abweichung von einer ehrlichen, verantwortungsbewussten Sprache.

2. Die Drei-Säulen-Analyse

Das Werkzeug identifiziert Muster, bei denen die Handlung im Text zwar bestehen bleibt, der Handelnde aber verschwindet.

Säule 1 (Inhaltliche Kritikalität): Fokus auf Stellen mit Fristen, Zahlen, Rechten/Pflichten oder Beendigungen.

Säule 2 (Stilbruch): Analyse, ob die Sprache an kritischen Stellen plötzlich von der restlichen Text-Basis abweicht (z. B. plötzliche Kälte).

Säule 3 (Distanzsprache): Messung der Entkopplung durch Passivkonstruktionen („wurde festgestellt“), unpersönliche Subjekte („es erfolgte“) und Nominalstil.

3. Methodik: Relatives Sprachrauschen

Um Fehlalarme zu vermeiden, arbeitet XACTDET mit einer relativen Messung:

Ein Merkmal (wie das Passiv) ist erst dann auffällig, wenn es an einer kritischen Stelle massiv häufiger auftritt als im restlichen Dokument (das „Delta“).

Kumulatives Prinzip: Ein Alarm (Rot) wird nur ausgelöst, wenn mehrere Säulen gleichzeitig anschlagen (z. B. Distanzsprache + Frist-Kontext).

4. Ergebnisausgabe (Farb-Semantik im Terminal)

Die Ausgabe erfolgt bewusst schlicht, um den Charakter als Analyse-Tool zu wahren:

Grün: Unauffällig im Rahmen des Textrauschens.

Gelb: Leichte Abweichungen; menschliche Prüfung empfohlen.

Rot: Signifikante Bündelung von Distanzmarkern an kritischen Stellen; starker Hinweis auf intentionale Verantwortungsminimierung.

5. Philosophische Einordnung

XACTDET reagiert auf das Problem der Selbstentlastung durch Grammatik. Es schützt den „Klugen“ vor der sprachlichen Vorfeldsicherung derer, die sich hinter Prozessen verstecken, um nicht persönlich für operative Fehler haften zu müssen. Es ist ein Verhinderungswerkzeug, das Transparenz schafft, wo Verantwortung sprachlich verdampft.

Status: Das Konzept ist fachlich und ethisch sauber, da es keine Urteile („Betrug“) fällt, sondern statistische Muster der Manipulation markiert

Fehler im Konzept: Wenn XACTDET nur auf Distanz prüft, entwischt der „warme Manipulator“.

Korrektur: Wir brauchen in der patterns.json auch „Pseudo-Empathie-Marker“. Wörter, die Verantwortung suggerieren, sie aber im nächsten Halbsatz durch ein „aber“ oder „wegen“ wieder auflösen (Kausalitäts-Check).
