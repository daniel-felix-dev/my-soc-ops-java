🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# ⭕ Soc Ops

> **Break the ice. Connect with strangers. Win at bingo.**

Soc Ops is a collaborative social bingo game designed for in-person mixers, conferences, and team events. Players find others who match custom prompts, mark squares, and race to complete five in a row. It's a modern take on an icebreaker—playful, low-pressure, and genuinely fun.

Perfect for:
- 🎓 **Conferences & Workshops** — Help attendees network with purpose
- 🏢 **Team Building** — Break down silos in a relaxed, game-oriented way
- 🎉 **Social Events** — Spark conversations at parties, mixers, and hangouts
- 🚀 **Community Gatherings** — Create memorable first interactions

---

## 🚀 Quick Start

**Option 1: Run Locally**

```bash
# Prerequisites: Java 21+ and Maven 3.9+
cd socops
./mvnw spring-boot:run
```

Open your browser to `http://localhost:8080` and start playing!

**Option 2: Deploy**

```bash
# Build and package
cd socops
./mvnw clean package

# Run the JAR
java -jar socops/target/*.jar
```

The app deploys automatically to GitHub Pages on every push to `main`.

---

## 📚 Learn & Customize

Soc Ops comes with a **comprehensive workshop guide** that teaches you to:

✅ Set up your development environment  
✅ Design a polished, distinctive frontend  
✅ Create custom Quiz Master agents  
✅ Orchestrate multi-agent workflows  

| Part | Focus |
|------|-------|
| [**00**](workshop/00-overview.md) | Overview & Setup Checklist |
| [**01**](workshop/01-setup.md) | Dev Environment & Context Engineering |
| [**02**](workshop/02-design.md) | Design-First Frontend Development |
| [**03**](workshop/03-quiz-master.md) | Custom AI Prompt Engineering |
| [**04**](workshop/04-multi-agent.md) | Multi-Agent Orchestration |

👉 **[Start the Full Lab Guide →](workshop/GUIDE.md)**

---

## 🛠️ Development

**Requirements:**
- Java 21 JDK ([Adoptium](https://adoptium.net/))
- Apache Maven 3.9+ (included via Maven Wrapper)

**Commands:**

```bash
# Run the app in development mode (with hot-reload)
cd socops && ./mvnw spring-boot:run

# Build a production package
cd socops && ./mvnw clean package

# Run tests
cd socops && ./mvnw test

# Format code & check for linting issues
cd socops && ./mvnw spotless:apply
```

---

## 🎮 How It Works

1. **Generate a board** — Each player gets a 5×5 grid of prompts (e.g., "Find someone with a tattoo", "Find a vegetarian", "Find someone who codes in Rust")
2. **Mingle & Mark** — Players move around finding others who match the squares
3. **Get Five in a Row** — First person to complete a line horizontally, vertically, or diagonally wins
4. **Repeat & Remix** — Swap in new prompts, new boards, infinite rounds

---

## 🔧 Architecture

**Stack:**
- **Backend:** Spring Boot 3.4.x with Java 21
- **Templates:** Thymeleaf
- **Styling:** Custom CSS utilities (no heavy frameworks)
- **Testing:** JUnit + Spring Boot Test

The codebase is lean and intentionally simple—great for learning, extending, and deploying at scale.

---

## 📄 License

This project is open source. See [LICENSE](LICENSE) for details.

---

**Ready to play? [Run it locally](#-quick-start) or [explore the workshop](workshop/GUIDE.md).**

