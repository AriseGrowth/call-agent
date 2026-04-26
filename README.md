# Whisper Transcription Service for Render

שירות תמלול פשוט מבוסס FastAPI + OpenAI.

## מה הוא עושה
- מקבל קובץ אודיו/וידאו
- שולח אותו לתמלול
- מחזיר טקסט מלא ב-JSON

## פורמטים נתמכים
- mp3
- mp4
- m4a
- wav
- mpeg
- mpga
- webm

## הרצה מקומית

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
export OPENAI_API_KEY=sk-xxxx
uvicorn main:app --reload
