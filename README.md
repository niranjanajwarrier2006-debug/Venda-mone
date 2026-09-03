# Venda Mone 🎯

## Basic Details

### Team Members
- Team Lead: Niranjana J Warrier - LBS Institute of Technology for Women

### Project Description
A chaotic cursor-tag simulator and psychological morality test where you chase an anxious virtual entity trying its best to avoid you. If you lack self-control and click it while it's begging for its life, you’re dragged straight into a gothic underworld jail under "Chaathan presiding"—complete with heavy iron bars, brutal sarcasm, and a mandatory apology letter that gets aggressively judged by the system. Show a little restraint and leave it alone, though, and you'll ascend straight to heaven to bask in lavish praises, karma ledgers, and respect scores. Packed with 20 unique unlockable creatures, a stunning Dark Academia glassmorphism UI, custom web audio soundscapes, and an embedded horror scream effect, it's the ultimate way to find out if you're actually a good person or just an absolute menace to digital wildlife.

### The Problem (that doesn't exist)
Humanity faces an urgent, completely fabricated crisis: how to test whether people have the basic moral restraint not to torment an innocent, anxious virtual creature. Society is plagued by the overwhelming urge to click things we have no business touching, leaving us with no lightweight, browser-based way to judge our own life choices.

### The Solution (that nobody asked for)
A chaotic cursor-tag simulator and psychological morality test where your choice to show restraint or give in to temptation decides your fate. Choose wisely and ascend to heaven for praise; give in, click the crying creature, and get dragged into a gothic underworld jail under "Chaathan presiding" to face heavy iron bars, brutal sarcasm, and a mandatory AI-judged apology letter. Complete with an 80-point collection of 20 paranoid pets, Dark Academia glassmorphism UI, custom web audio soundscapes, and an embedded horror scream, it is the ultimate tool to prove whether you are a good person or an absolute menace.

## Technical Details
### Technologies/Components Used
For Software:
- HTML5
- Tailwind CSS (via CDN)[cite: 2]
- Vanilla JavaScript[cite: 2]
- Web Audio API & Base64 Audio Data URIs[cite: 2]

For Hardware:
- Standard student laptop/desktop computer
- Standard mouse or cursor input device

### Implementation
For Software:
# Installation
```bash
# Clone the repository or download the source code
git clone [https://github.com/niranjanajwarrier2006-debug/venda-mone.git](https://github.com/niranjanajwarrier2006-debug/venda-mone.git)

# Navigate into the project folder
cd venda-mone
To Run:
# Open index.html directly in any modern web browser or run via VS Code Live Server
start index.html

Project Documentation
For Software:
Screenshots



![alt text](<Screenshot 2026-09-04 033629-1.png>)
![alt text](<Screenshot 2026-09-04 033704.png>)
![alt text](<Screenshot 2026-09-04 033714.png>)
![alt text](<Screenshot 2026-09-04 033727.png>)
![alt text](<Screenshot 2026-09-04 033805.png>)
![alt text](<Screenshot 2026-09-04 033854.png>)

Diagrams
[ Start / Idle State ]
         │
         │ (Cursor approaches / distance drops)
         ▼
    [ Fleeing State ]
         │
         ├── (Panic threshold / rapid movement) ──► [ Panic State ]
         │                                              │
         └── (Energy drained / depletion) ◄─────────────┘
                         │
                         ▼
                [ Exhausted State ]
         (7-second countdown + pleading dialogue)
                         │
          ┌──────────────┴──────────────┐
          │                             │
    (Player clicks)             (Timer reaches 0)
          │                             │
          ▼                             ▼
   [ Hell Outcome ]             [ Heaven Outcome ]
- Chaathan Presiding         - Karma Ledger & Titles
- Heavy Iron Bar Jail        - Respect Score Bar
- Heuristic Apology Trial    - Sincere Compliments
- Unlock Points Banked       - Creature Unlock System

stateDiagram-v2
    direction TB
    
    [*] --> Idle: Game Starts
    
    Idle --> Fleeing: Cursor Approaches
    Fleeing --> Panic: Rapid Evasion / High Speed
    Panic --> Exhausted: Energy Depleted (0-100)
    Fleeing --> Exhausted: Energy Depleted (0-100)
    
    state Exhausted {
        [*] --> PleadingDialogue: 7-Second Countdown Begins
    }

    Exhausted --> HellOutcome: Player Clicks (Moral Failure)
    Exhausted --> HeavenOutcome: Timer Reaches 0 (Restraint Shown)

    state HellOutcome {
        [*] --> ChaathanPresiding
        ChaathanPresiding --> IronBarJail
        IronBarJail --> HeuristicApologyTrial
    }

    state HeavenOutcome {
        [*] --> KarmaLedger
        KarmaLedger --> RespectScoreBar
        RespectScoreBar --> CreatureUnlockSystem
    }

    HellOutcome --> [*]
    HeavenOutcome --> [*]


Project Demo
Video
https://drive.google.com/file/d/1JQjEhVraLXAg7KMMg01qbdxDtQ9BzG97/view?usp=sharing
Demonstrates the full gameplay loop, creature evasion, collection unlocks, and audio integration[cite: 2].


Team Contributions
Niranjana J Warrier: Solo development — handled everything from core game logic, state machine architecture, and movement mechanics to the apology evaluation algorithm, creature collection system, Dark Academia UI/UX styling, and Web Audio/Base64 sound integration[cite: 2].

Made with ❤️ at TinkerHub Useless Projects

