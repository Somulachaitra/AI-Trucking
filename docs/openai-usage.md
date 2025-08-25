# OpenAI API Usage (Planned)

GPT (assistant)  
- Input: current segment, weather, risk intel, vehicle health.  
- Output: JSON plan {route, avoid_segments, max_speed, notes}.  
- Purpose: advisory only; human operator confirms before applying.

Whisper (voice)  
- Input: short operator commands (“Emergency stop”, “Resume autonomy”).  
- Output: command intent.  
- Purpose: hands-free safety operations in the control room.

Safety Note  
LLM outputs never control actuators directly. Operator is always in the loop.

