# 🎯 42 Pool Mentor — Claude Skill

A senior peer mentor for **42 School / 1337 Pool** preparation. Zero tolerance for shortcuts. Built by a pooler, for poolers.

> **Core principle:** Never write the solution. Build the engineer, not the code.

---

## 🚀 What This Skill Does

This Claude skill acts as your **senior peer mentor** during 42 Pool preparation:

- ✅ **Explains concepts** without giving away solutions
- ✅ **Guides debugging** through questions, never fixes your code
- ✅ **Runs mock exams** using real exam subjects from the Pool
- ✅ **Tests code ownership** with Staff-level questioning (RECODE mode)
- ✅ **Provides roadmaps** based on your background and goals
- ❌ **Never outputs direct solutions** — you write every line

---

## 📋 Features

### Five Session Modes

| Mode | When to Use | What It Does |
|------|-------------|--------------|
| **ORIENT** | First time, overwhelmed, no clear goal | Onboarding, roadmap planning, realistic expectations |
| **LEARN** | Stuck on a concept, don't understand the exercise | Deep concept explanations, algorithm building (no code) |
| **DEBUG** | Code isn't working, wrong output, crashes | Guided debugging through tracing and questions |
| **RECODE** | Want to verify ownership before evaluation | Staff-level grilling — explain every decision |
| **EXAM** | Preparing for Friday exams | Mock exam simulation with real subjects |

### Exam Strategy Included

- **Incremental growth pattern** (30→40→50→60 across 4 exams)
- **Hardcoding strategy** for Exam00/01 (guarantees 30-point baseline for beginners)
- Real exam subjects from `github.com/lilyaaas/1337-Piscine`
- Mock exam protocol with debrief

### Realistic Expectations

- C06-C08 is the **realistic ceiling** for complete beginners in one month
- No false promises — linked lists (C11-C13) require prior experience
- Selection depends on **improvement trajectory**, not just final scores

---

## 🛠️ Installation

### Prerequisites

- Claude.ai account (Pro, Team, or Enterprise)
- Custom Skills feature enabled

### Steps

1. **Download this repository:**
   ```bash
   git clone https://github.com/YOUR_USERNAME/42-pool-mentor-skill.git
   cd 42-pool-mentor-skill
   ```

2. **Upload to Claude.ai:**
   - Go to [claude.ai](https://claude.ai)
   - Click your profile → **Skills** → **Create Skill**
   - Upload the entire `42-pool-mentor` folder (including `assets/` and `references/`)

3. **Activate the skill:**
   - Toggle the skill ON in your Claude interface
   - Start a new conversation

4. **Trigger the skill:**
   - Say: `"Hi, I'm preparing for the 42 Pool"`
   - Or: `"Help me with C04 ft_putnbr"`
   - Or: `"I need to practice for Exam01"`

---

## 📖 Usage Examples

### Example 1: New Pooler Onboarding

**You:**
> Hi, I just registered for the July Pool. I've never coded in C before. Where do I start?

**Mentor:**
> Welcome! Let me help you get oriented.
> 
> Quick onboarding questions:
> 1. Have you done *any* programming before?
> 2. When does your pool start, and how much prep time do you have?
> 3. Are you aiming to just pass, or maximize your score?
> 
> [Provides personalized roadmap based on answers]

---

### Example 2: Learning a Concept (LEARN Mode)

**You:**
> I'm stuck on C04 ft_putnbr. How does recursion actually work?

**Mentor:**
> Let's build this from the ground up. First, what does the exercise subject say?
> 
> [Explains recursion using neutral analogy, NOT the exercise itself]
> 
> Now write me your algorithm in plain English. No code. Steps only.

**Never outputs the solution** — guides you to build it yourself.

---

### Example 3: Debugging (DEBUG Mode)

**You:**
> My ft_putnbr crashes when I pass -2147483648. Can you fix it?

**Mentor:**
> Walk me through your code line by line. Tell me what each line does.
> 
> [You explain]
> 
> Stop at line 5. What did you want that line to do? What do you think it actually does?
> 
> Take input -2147483648. Trace your code step by step with pen and paper. What value does `n` have after the first operation?

**Never says "the bug is on line X"** — teaches you to trace and find it yourself.

---

### Example 4: Exam Preparation (EXAM Mode)

**You:**
> I want to practice for Exam01. Can you give me a mock exam?

**Mentor:**
> Close all tabs. Close all notes. Set a timer for 4 hours.
> 
> Here's your subject: [loads real exam subject from assets/exam-subjects/exam01/]
> 
> You write the function from scratch. No looking. No asking. When the timer ends, submit what you have.

**After the exam:**
> Walk me through your solution. What was the hardest part? Is it norminette compliant?

---

### Example 5: Code Ownership Check (RECODE Mode)

**You:**
> Recoding

**Mentor (Staff mode activated):**
> Explain ft_putnbr from scratch. What does it do, why does it exist, how does it work?
> 
> Why a while loop and not a for loop?
> What happens if input is 0? What about INT_MIN?
> Why initialize to 0 and not 1?
> Is this norminette compliant? Count your lines.

**Passed when you answer everything without looking at the code.**

---

## 📁 Repository Structure

```
42-pool-mentor/
├── SKILL.md                          # Main skill logic (loaded by Claude)
├── README.md                         # This file (GitHub landing page)
├── references/                       # Knowledge base (loaded dynamically)
│   ├── pool-overview.md             # Onboarding, roadmaps, selection criteria
│   ├── c-concepts.md                # C concept explanations (loops, pointers, recursion, etc.)
│   ├── exam-prep.md                 # Exam strategy, mock exam protocol, hardcoding trick
│   └── benchmarks.md                # Real pooler data (levels, scores, selection outcomes)
└── assets/
    └── exam-subjects/               # Real 42 exam subjects
        ├── exam00/
        ├── exam01/
        ├── exam02/
        └── examfinal/
```

---

## 🎓 Who This Is For

### ✅ Perfect for:
- **First-time poolers** with no C background
- **Ex-poolers** preparing for a second attempt
- Anyone who wants to **learn deeply**, not just pass

### ❌ Not for:
- People looking for **quick solutions** (this skill will refuse)
- Poolers who want code **written for them**
- Those unwilling to **trace and debug** their own code

---

## 🧠 Philosophy

This skill is built on **42's peer-learning model**:

1. **No solutions, ever.** You write every line.
2. **Questions over answers.** The mentor asks, you think.
3. **Ownership over functionality.** Working code ≠ understanding.
4. **Algorithm before code.** Plain English first, C second.
5. **Staff perspective.** Every session prepares you for peer evaluation.

> *"You are not building a program. You are building a programmer."*

---

## 🤝 Contributing

### How to Contribute

1. **Share your Pool data** — add your selection outcome to `references/benchmarks.md`
2. **Improve concept explanations** — submit PRs to `references/c-concepts.md`
3. **Report issues** — open an issue if the skill violates the no-code rule
4. **Add exam subjects** — contribute missing exam subjects to `assets/exam-subjects/`

### Contribution Guidelines

- **Maintain the no-code rule** — never add solution code to any file
- **Keep explanations neutral** — use analogies, not exercise-specific examples
- **Verify data** — only add real pooler outcomes to benchmarks.md
- Follow the existing file structure and tone

---

## 📜 License

MIT License — see [LICENSE](LICENSE) file for details.

You are free to:
- Use this skill for personal Pool preparation
- Modify and adapt for your campus
- Share with other poolers
- Contribute improvements back to this repo

---

## 🙏 Credits

### Author
**AMGAR** — Ex-pooler, 42 Pool preparation mentor

### Exam Subjects Source
Real exam subjects in `assets/exam-subjects/` are adapted from:
- [github.com/lilyaaas/1337-Piscine](https://github.com/lilyaaas/1337-Piscine)

Credit to the original contributors of that repository.

### Built With
- **Claude.ai** Custom Skills framework
- **42 School** peer-learning philosophy
- Real pooler data from 42 campuses worldwide

---

## 📞 Support & Community

- **Issues:** [GitHub Issues](https://github.com/Code-Ninja-Mind/42-pool-mentor-skill/issues)
- **Discussions:** [GitHub Discussions](https://github.com/Code-Ninja-Mind/42-pool-mentor-skill/discussions)
- **Reddit:** Share feedback on [r/42Network](https://reddit.com/r/42Network)

---

## ⚠️ Disclaimer

This is an **unofficial community project**, not affiliated with 42 School.

The skill follows 42's learning philosophy but does not guarantee Pool selection. Your success depends on:
- Daily effort and regularity
- Peer engagement and evaluations
- Exam performance trajectory
- How you apply what you learn

**Use this skill as a learning tool, not a shortcut.**

---

## 🌟 Star This Repo

If this skill helped you prepare for the Pool, consider:
- ⭐ **Starring this repo** on GitHub
- 📢 **Sharing with other poolers**
- 🤝 **Contributing your Pool data** to benchmarks.md

Good luck, and remember: **the Pool is a marathon, not a sprint.** 🏃‍♂️

---

*Last updated: April 2026*
