# OpenAI API Usage (Planned)

This document explains how **GPT** and **Whisper** are integrated into the AI-Trucking prototype.  
⚠️ **Note:** AI outputs are *advisory only*. Operators always confirm actions before execution. No model output directly controls actuators.

---

## 🧠 GPT (Assistant)

**Purpose:** Provides **risk-aware routing advice** based on context.  
**Input:** current segment, weather, risk intelligence, vehicle health.  
**Output:** JSON advisory plan (operator validates before use).

### Example Input
```json
{
  "segment": "Highway-19",
  "weather": "Heavy rain",
  "risk_intel": "Flood warning ahead",
  "vehicle_health": "OK"
}
```
### Example Output
```json
{
  "route": "Highway-47 → City Bypass → Safe Depot",
  "avoid_segments": ["Highway-19 flood zone"],
  "max_speed": 60,
  "notes": "Storm risk near Segment-3, reroute advised"
}
```
## 🎙️ Whisper (Voice)

**Purpose:** Enables hands-free emergency commands in the control room.  
**Input:** Short operator phrases(e.g., “Emergency stop”, “Resume autonomy”).

**Output:** Command intent mapping.


## Example Input (spoken)
``` arduino
"Emergency stop"
```
## Example Output
``` json
{
  "command": "STOP"
}
```
## Another Example Input (spoken)
``` arduino
"Resume autonomy"

```
## Example Output
``` json
{
  "command": "RESUME_AUTONOMY"
}
```
---
## 🔐 Safety Note

* All AI outputs are filtered + validated before being shown to operators.
* Operator must approve any reroute or action.
* AI is an advisor, not a driver.

## 📌 Summary

* GPT: Generates JSON routing plans → operator decides.
* Whisper: Maps voice commands → operator confirms.
* Operator: Always in control.


