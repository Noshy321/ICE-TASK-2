# CyberGuard - Cybersecurity Awareness Chatbot
## PROG6221 Part 1 | Console Application

---

## Project Description

CyberGuard is a command-line cybersecurity awareness chatbot developed for South African citizens. The chatbot educates users about online safety practices including password security, phishing detection, safe browsing, and scam prevention. This is Part 1 of a three-part POE submission.

---

## Features

| Feature | Description |
|---------|-------------|
| Voice Greeting | Plays WAV audio at startup |
| ASCII Art Logo | Custom cybersecurity-themed logo |
| Personalised Interaction | Asks for and remembers user's name |
| Keyword Recognition | Responds to cybersecurity topics |
| Input Validation | Handles empty or invalid inputs |
| Help System | Displays available commands |
| Typing Animation | Natural conversation simulation |
| Coloured Console | Cyan, green, red, yellow text |
| Security Threat Meter | Animated threat level display |

---

## Topics Covered

- Password safety
- Phishing scams
- Safe browsing
- Privacy protection
- Online scams
- South African cybersecurity statistics

---

## Commands

| Command | Action |
|---------|--------|
| `help` | Display help menu |
| `joke` | Tell a cybersecurity joke |
| `tip` | Give a security tip |
| `exit` or `bye` | Exit the chatbot |

### Example Questions
How do I create a strong password?
What is phishing?
How to browse safely?
Tell me about privacy

text

---

## Requirements

| Requirement | Version |
|-------------|---------|
| .NET SDK | 8.0 or higher |
| Visual Studio | 2022 |
| Operating System | Windows 10/11 |

---

## Installation and Setup

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/CybersecurityChatbot.git
cd CybersecurityChatbot
Step 2: Build the Project
bash
dotnet build
Step 3: Run the Application
bash
dotnet run
Step 4: Audio Setup (Optional)
Place your greeting.wav file in:

text
CybersecurityChatbot/bin/Debug/net8.0/greeting.wav
If no WAV file is found, the application uses console beeps as a fallback.

Project Structure
text
CybersecurityChatbot/
├── Program.cs                 # Entry point
├── Models/
│   └── Chatbot.cs            # Main chatbot logic
├── Services/
│   ├── AnimationService.cs   # Typing and loading effects
│   ├── ResponseEngine.cs     # Keyword detection
│   ├── SoundService.cs       # Audio playback
│   └── ThreatLevelMonitor.cs # Suspicious keyword detection
├── Utilities/
│   ├── AsciiArtGenerator.cs  # ASCII logo display
│   ├── JokeLibrary.cs        # Jokes collection
│   └── UiHelper.cs           # Colours and borders
├── Data/
│   └── CybersecurityFacts.cs # SA statistics and tips
├── Resources/
│   └── greeting.wav          # Voice greeting file
└── README.md                 # This file
GitHub and CI Setup
Commits
The repository contains a minimum of 6 meaningful commits with descriptive messages:

text
- Initial commit: Project structure
- Added ASCII art and voice greeting
- Implemented response engine
- Added UI helper with colours
- Added help menu and commands
- Final cleanup and CI setup
Continuous Integration
GitHub Actions is configured to automatically build and verify the code on each push.

CI Workflow Status:

https://screenshots/ci-success.png

Screenshot showing green check mark from GitHub Actions

Video Presentation
An unlisted YouTube video demonstrating:

Code structure explanation

Live application demo

Logic and flow explanation

Voice integration and formatting techniques

Video Link: Click here to watch

Assessment Criteria Met
Criteria	Status
Voice Greeting and Image Display	✅
Greeting and User Interaction	✅
Basic Response System	✅
Input Validation	✅
Enhanced Console UI	✅
Code Structure and Readability	✅
GitHub and CI Setup	✅
Video Presentation	✅
Correct Submission	✅
References
Pieterse, H. 2021. The Cyber Threat Landscape in South Africa: A 10-Year Review. The African Journal of Information and Communication, 28(28). doi: https://doi.org/10.23962/10539/32213

Author Information
Detail	Information
Name	[Your Full Name]
Student Number	[Your Student Number]
Module	PROG6221 - Programming 2A
Assessment	POE Part 1
Date	2026
Troubleshooting
Issue	Solution
No sound at startup	Place greeting.wav in output directory
ASCII art misaligned	Set console font to Consolas
Build fails	Run dotnet restore
Stay safe online. CyberGuard is here to help. 🔒

text

---

## 📝 Instructions to Complete

Replace these placeholders before submitting:

| Placeholder | Replace With |
|-------------|--------------|
| `YOUR_USERNAME` | Your GitHub username |
| `YOUR_VIDEO_LINK` | Your unlisted YouTube video URL |
| `[Your Full Name]` | Your actual name |
| `[Your Student Number]` | Your student ID |

---

## 📸 Add CI Screenshot

1. Create a folder called `screenshots` in your repository
2. Go to GitHub → Actions tab
3. Click on a successful workflow run (green check mark)
4. Take a screenshot
5. Save as `ci-success.png` in the `screenshots/` folder
6. Commit and push

---

## ✅ Before Submitting

- [ ] Replace all placeholders with your actual information
- [ ] Add CI screenshot
- [ ] Upload video to YouTube (unlisted)
- [ ] Paste YouTube link in README
- [ ] Commit and push to GitHub
- [ ] Submit GitHub link on ARC

Would you like me to help with the **GitHub Actions workflow file** or **video presentation script** next?
