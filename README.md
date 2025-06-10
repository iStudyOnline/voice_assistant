# voice_assistant
Voice assistant linking the user with a chat service through speech-to-text and text-to-speech

## THIS YAH Verify

`this_yah_verify/verify_agent.py` provides a command line tool to verify claims using open-source information. It searches DuckDuckGo, BAILII and Archive.org, performs basic named-entity recognition and can export reports as JSON or DOCX.

### Setup

```bash
pip install -r requirements.txt
python -m spacy download en_core_web_sm
```

### Usage

```bash
python -m this_yah_verify.verify_agent "Is this video real?" \
  --media-url https://example.com/video.mp4 --export-json report.json
```

Network access is required for searches and media checks.
