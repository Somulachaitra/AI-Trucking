# AI-Trucking 🚛🛰️  
*A satellite-supervised, AI-assisted trucking system (digital prototype)*

---

## 🌍 What it is
AI-Trucking is a **satellite-supervised, AI-assisted trucking system** that keeps drivers out of danger by enabling:
- **Remote monitoring** from a central control room  
- **Risk-aware rerouting** using AI + satellite intel  
- **Tele-operation fallback** during climate or security risks  

---

## ❓ Why it matters
Trucking is **dangerous in many regions** due to:
- Extreme weather 🌪️  
- Robbery and roadside attacks 🛑  

Our prototype shows how **AI + satellite oversight** can keep supply chains moving **while protecting human lives**.  

---

## 📂 What this repo contains
- `design/` → system diagrams, dashboard mockups, and the one-pager  
- `docs/` → evaluation notes and OpenAI API usage plan  
- `README.md` → project overview (this file)

---
## 🚀 Getting Started

### Prerequisites

* [Git](https://git-scm.com/)
* [Python 3.9+](https://www.python.org/)
* [Jupyter Notebook](https://jupyter.org/) (for experiments)

### Installation

```bash
# Clone the repo
git clone https://github.com/Somulachaitra/AI-Trucking.git
cd AI-Trucking

# (Optional) Setup virtual environment
python -m venv venv
source venv/bin/activate   # For Linux/Mac
venv\Scripts\activate      # For Windows

# Install dependencies
pip install -r requirements.txt
```

### Running the Project

```bash
python main.py
```


---

## 🧠 OpenAI API Usage
We use OpenAI models as **decision support only** — never for direct actuation.

### GPT (assistant)
- **Input:** `{segment, weather, risk intel, vehicle health}`  
- **Output (example):**
```json
{
  "route": "Highway-47 → City Bypass → Safe Depot",
  "avoid_segments": ["Highway-19 flood zone"],
  "max_speed": 60,
  "notes": "Storm risk near Segment-3, reroute advised"
}
```

## 🏗️ System Architecture

Here’s how the system works:

![System Architecture](design/system-diagram.png)

* **Data Layer** → Stores trip & fuel data.
* **AI Engine** → Runs optimization and predictions.
* **Visualization** → Displays results in dashboards.
* **User Interface** → Simple interface for interactions.

---

## 📂 Project Structure

```
AI-Trucking/
│── docs/                   # Documentation
│   ├── evaluation-fit.md
│   ├── openai-usage.md
│── design/                 # Design diagrams
│   ├── system-architecture.md
│   ├── one-pager.pdf
│── README.md               # Project introduction
```
---

## 📊 Evaluation

We measure performance using:

* ✅ **Route optimization accuracy**
* ✅ **Fuel efficiency improvement**
* ✅ **Time saved per trip**

---

## 📘 Documentation

* [One-Pager](design/one-pager.pdf)
* [System Architecture](design/system-architecture.md)
* [Evaluation Fit](docs/evaluation-fit.md)
* [OpenAI Usage](docs/openai-usage.md)

---

## 🌱 Future Scope

* 🚀 Real-time GPS integration
* 📡 IoT sensors for truck monitoring
* 🔒 Blockchain for secure logistics data
* 🌍 Scaling AI to multi-city fleets

---

## 🙋‍♂️ About Me

Hi 👋, I’m **Chaitra Somula**, a **2nd-year B.Tech student** passionate about **AI and Systems Engineering**.
This project is a step towards applying classroom learning to **real-world logistics challenges**.

📧 Contact: \[[schaitra3894@gmail.com](mailto:schaitra3894@gmail.com)]
🔗 GitHub: [Somulachaitra](https://github.com/Somulachaitra)

---

⭐ If you liked this project, don’t forget to **star the repo**!

