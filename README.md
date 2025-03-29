# 🧠 Legendary AI Calendar Assistant

A no-code, AI-powered calendar assistant that schedules events via chat using **n8n**, **OpenAI**, and **Google Calendar**.  
Say goodbye to manual scheduling — just type, and your assistant handles the rest.

---

## ✨ What This Project Does

This project automates scheduling in your calendar using natural language:

- 🗓️ Reads your availability from **Google Calendar**
- 💬 Accepts natural chat commands like "Book a meeting at 10AM tomorrow"
- 🧠 Uses **OpenAI GPT-4o-mini** to understand your intent and extract times
- 🤖 Schedules the event if the time is free
- 🧩 Built using **n8n** – a powerful no-code workflow builder

---

## 🎯 Why I Built This

I created this project as part of my transition from **Software Engineer** to **Technology Consultant**, to showcase how AI can enhance productivity through automation.

My goals were to:
- Learn how to design and deploy **AI workflows** using no-code tools
- Practice **prompt engineering** and dynamic system messages
- Demonstrate how consultants can build internal tools without code
- Explore human-like interaction with calendar agents

---

## 🧪 Tech Stack

| Layer         | Tool                     | Purpose                                  |
|--------------|--------------------------|------------------------------------------|
| Workflow      | [n8n](https://n8n.io)     | No-code automation platform              |
| AI Model      | OpenAI GPT-4o-mini       | Extracts times and context from prompts  |
| Calendar Tool | Google Calendar API      | Creates events and checks availability   |
| Trigger       | Chat Interface (n8n)     | Accepts user requests                    |

---

## 🖼️ Screenshots

| Workflow Setup | Working Agent |
|----------------|---------------|
| ![Workflow](./assets/Screenshot-setup.png) | ![Agent Booking](./assets/Screenshot-booking-success.png) |

| Fun Prompt Interaction |
|------------------------|
| ![Fun](./assets/Screenshot-fun-prime-rule.png) |

> All screenshots taken from my working setup — see `/assets` folder for more.

---

## ⚙️ How It Works

1. **User types a request** into the n8n chat (e.g., _"Book a meeting tomorrow at 10AM"_)
2. The **OpenAI chat model** parses intent, extracts start & end times
3. n8n’s **AI Agent node** passes those times to the **Google Calendar node**
4. If the time is available, the event is created — else the assistant suggests alternatives

---

## 🔍 What I Learned

| Area | Takeaways |
|------|-----------|
| **AI Workflow Design** | Trigger → AI Model → Action pattern |
| **Prompt Engineering** | Writing effective system messages |
| **n8n** | Connecting nodes, debugging with logs |
| **Google API** | OAuth setup and event creation |
| **Debugging** | Dynamic date/time injection and troubleshooting AI responses |

---

## 📅 Unique Features

✅ Bookings only on **even-numbered days**  
✅ Events start at **prime-numbered minutes only**  
✅ Mood-check interaction before scheduling  
✅ Fully configurable **system message personality**  
✅ Uses your **real Google Calendar** session

---

## 💡 Example Prompts

```text
Can I schedule a meeting for tomorrow at 10AM?
I’m in the mood for a call – book me something at 4PM on Friday.
Let’s meet next Wednesday at noon called ‘Strategy Sync’.

---

## 🚀 How To Run

This project was built using **n8n Cloud** (14-day free trial).  
✅ **No code required.**

👉 See the original tutorial [here](https://www.nextwork.org/) to get started with your own AI workflows.

---

## 🙌 Acknowledgements

Special thanks to the team at **NextWork** for the original walkthrough and challenge idea.  
This project extends and customizes their tutorial to fit my personal learning goals and AI consulting portfolio.

---

## 📚 License

This project is licensed under the **MIT License**.  
See the [LICENSE](./LICENSE) file for full details.

---

## 🧑‍💻 Author

**Edouardos Stavrakis**  
Technology Consultant & AI Enthusiast  
[LinkedIn](https://www.linkedin.com/in/edouardosstavrakis/) | [GitHub](https://github.com/EdouardosStav)

---

## ⭐ Like It?

Give this repo a ⭐ and fork it to build your own AI calendar assistant!

