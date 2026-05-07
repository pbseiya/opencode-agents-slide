# Prometheus Plan: Detailed Thai Narration for OpenCode Slide Deck

## Context
Project: ~/projects/opencode-agents-slide/
Files: index.html (10 slides), content.md (Thai content), audio/ (existing .ogg files)

## Objective
Replace all 10 audio narration files with much more detailed, comprehensive Thai narration that explains each concept thoroughly like a real instructor.

## Execution Steps (Atlas to execute)

1. Read current content.md and index.html to ensure content alignment
2. Write narration-scripts.md containing detailed Thai scripts for all 10 slides
   - Each script: 30-60 seconds of speech, educational tone, natural Thai
   - Explain concepts deeply, give examples, analogies
3. Generate audio via text_to_speech for slide-01 through slide-10
   - Output paths: ~/projects/opencode-agents-slide/audio/slide-XX.ogg
4. Verify all 10 audio files exist and have reasonable size
5. Git commit and push

## Slide Narration Outline

Slide 1 (Intro): Greeting + what the deck covers + why it matters
Slide 2 (Why know agents?): Detailed explanation of cost/time savings vs waste
Slide 3 (Agent hierarchy): Deep dive into 3-tier system with analogies
Slide 4 (Golden rule): Explain delegation principle with company hierarchy analogy
Slide 5 (Sisyphus): Detailed use cases, when to use, ultrawork explained
Slide 6 (Prometheus): Step-by-step interview process, why planning matters
Slide 7 (Hephaestus): Deep reasoning scenarios, signals to call this agent
Slide 8 (Decision table): Walk through each scenario with examples
Slide 9 (Don't do): Anti-patterns explained with consequences
Slide 10 (Summary): Three-tier summary with encouragement
