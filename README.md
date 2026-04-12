# CyberGuard

A command-line cybersecurity awareness chatbot for South African citizens.

---

## What it does

CyberGuard educates users about online safety through conversation. It covers password security, phishing scams, safe browsing, and privacy protection. The bot remembers your name, responds to questions, and provides security tips.

---

## Features

- Voice greeting on startup (WAV file)
- ASCII art logo
- Personalised responses using your name
- Keyword detection for cybersecurity topics
- Typing animation and coloured console output
- Security threat level meter
- Help menu with available commands

---

## Commands

| Command | What it does |
|---------|---------------|
| `help` | Shows available commands and topics |
| `joke` | Tells a cybersecurity joke |
| `tip` | Gives a random security tip |
| `exit` or `bye` | Closes the application |

You can also ask questions like:

- "How do I create a strong password?"
- "What is phishing?"
- "How to browse safely?"
- "Tell me about privacy"

---

## Running the application

1. Open the solution in Visual Studio 2022
2. Build the project (Build > Build Solution)
3. Press F5 to run

If you want the voice greeting, place a `greeting.wav` file in the output folder (`bin/Debug/net8.0/`). The application will still run without it using console beeps.

---

## Project structure
CybersecurityChatbot/
├── Program.cs
├── Models/
│ └── Chatbot.cs
├── Services/
│ ├── AnimationService.cs
│ ├── ResponseEngine.cs
│ ├── SoundService.cs
│ └── ThreatLevelMonitor.cs
├── Utilities/
│ ├── AsciiArtGenerator.cs
│ ├── JokeLibrary.cs
│ └── UiHelper.cs
├── Data/
│ └── CybersecurityFacts.cs
└── Resources/
└── greeting.wav

text

---

## GitHub

This repository contains:

- Minimum 6 commits with descriptive messages
- GitHub Actions workflow for CI
- Build verification on each push

CI workflow status: **Passing**

![CI workflow screenshot](screenshots/ci-success.png)

---

## Reference

Pieterse, H. 2021. The Cyber Threat Landscape in South Africa: A 10-Year Review. *The African Journal of Information and Communication*, 28(28).
