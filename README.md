# AI Long Movie Generator

Generate long-form cinematic AI movies scene-by-scene.

## Features
- Break full scripts into scenes
- Generate AI video clips per scene (Sora, Runaway, etc.)
- Generate TTS narration and background music
- Stitch clips into a full-length movie
- Post-process for color, style, and continuity

# Folder Structure
See `file_tree.txt` for organized folders.

# How to use
1. Install dependencies: `pip install -r requirements.txt`
2. Configure API keys in `config/config.yaml`
3. Add your movie script in `assets/scripts/`
4. Run `scene_breaker.py` → `video_generator.py` → `audio_generatorn.py` → `video_stitcher.py`
5. Export final movie in `outputs/final/`

See `GUIDELINES.md` for detailed instructions for directors.
