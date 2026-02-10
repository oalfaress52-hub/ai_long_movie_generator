# AI Long Movie Generator — Guidelines for Filmmakers

This document provides best practices and instructions for using the AI Long Movie Generator to create **scene-by-scene cinematic movies**. It is aimed at directors, storytellers, and creatives who want to combine AI generation with traditional filmmaking control.

---

## 1️⃣ Project Purpose

- Generate AI-assisted cinematic movies from a **full script**.
- Maintain **visual consistency, narrative flow, and audio synchronization**.
- Modular pipeline: generate, edit, and stitch **scene clips**.

---

## 2️⃣ Workflow Overview

1. **Prepare Script**
   - Write your movie script in `assets/scripts/full_movie_script.txt`.
   - Include **scene headings, action, camera direction, mood, and style**.
   - For historical or notable figures (religious, cultural, or historical), **avoid direct human depiction**. Use **symbolism, abstract representations, or lighting effects** to show presence respectfully.

2. **Break into Scenes**
   - Run `scripts/scene_breaker.py` to segment the script into sub-scenes.
   - Configure scene duration, style, and cinematic notes in `config/scene_settings.json`.

3. **Generate Video Clips**
   - Run `scripts/video_generator.py` to generate AI clips per scene.
   - Use **clear cinematic prompts** specifying:
     - Camera angle: wide, close-up, tracking
     - Lighting: day, night, dramatic, soft
     - Mood: tense, epic, serene, suspenseful
     - Style: cinematic realism, epic, artistic filters
   - Ensure **negative prompts** for unwanted elements (faces, gore, logos, modern items).

4. **Generate Audio**
   - Run `scripts/audio_generator.py` to produce TTS narration.
   - Add **background music** and subtle sound effects.
   - Keep narration **consistent** (voice, pacing, tone).

5. **Stitch Scenes**
   - Use `scripts/video_stitcher.py` to combine clips into the full movie.
   - Verify **transitions**, **pacing**, and **continuity**.

6. **Post-Processing**
   - Optional: color grading, upscaling, stabilization (`scripts/post_process.py`).
   - Review final output for **visual and audio consistency**.

---

## 3️⃣ Prompt Guidelines

- **Clarity & brevity:** Keep prompts concise (2–5 sentences) but descriptive.
- **Consistency:** Use repeated descriptors (lighting, props, character style) across scenes.
- **Respectful depiction:** For historical, cultural, or religious figures, **avoid showing faces or human depictions** that could be inaccurate or disrespectful. Use **symbolism, abstract imagery, or lighting effects** instead.
- **Mood & cinematic direction:** Include tension, awe, serenity, or epic tone as needed.
- **Negative prompts:** Explicitly exclude unwanted features such as modern clothing, gore, text, logos, or faces if necessary.

---

## 4️⃣ Scene Planning Recommendations

- **Clip length:** 10–30 seconds per AI-generated clip for best quality.
- **Epic sequences:** Break into multiple clips to maintain smooth motion.
- **Overlap scenes:** Use transitional frames to make long sequences appear continuous.
- **Track visual continuity:** Ensure lighting, props, and camera angles remain consistent.

---

## 5️⃣ Audio & Music Guidelines

- Narration should **match scene length** and pacing.
- Background music should **enhance mood** without overpowering narration.
- Use **consistent TTS voice** for all narration.
- Sound effects should be **subtle and cinematic**.

---

## 6️⃣ Post-Production Tips

- Check **color grading** across clips.
- Ensure **lighting and style** continuity.
- Apply **smooth transitions**: fades, cross-dissolves, or wipes.
- Adjust **scene length** if pacing feels off.
- Review the **full movie** for clarity and flow.

---

## 7️⃣ Best Practices for Directors

- **Storyboard first:** Visual planning before AI generation improves consistency.
- **Test a single scene:** Refine style and prompts before generating full movie.
- **Organize assets:** Keep scripts, prompts, reference frames, clips, and audio in designated folders.
- **Iterate:** AI is experimental—multiple generations may improve quality.
- **Maintain logs:** Track which prompts produce best results for consistency.

---

## 8️⃣ Limitations

- AI may produce minor glitches or repetition.
- Maximum clip length is limited (~10–30 seconds per generation).
- Full-length movie requires **stitching multiple clips**.
- AI cannot fully guarantee perfect motion continuity for very long sequences.

---

✅ **Directors’ Tip:** Treat this as a **hybrid filmmaking tool**. AI generates raw cinematic assets, but human direction ensures storytelling, pacing, and cinematic quality.
