# Architecture

## High-Level System

Slides (PDF/PPT)
→ Upload API
→ Document Parser
→ Text Cleaner
→ Concept Extractor
→ Quiz Generator
→ Quiz JSON Output
→ Android App

## Main Components

### Backend
- Upload handling
- Slide/document parsing
- Concept extraction
- Quiz generation
- API layer
- Storage/database

### Android App
- Quiz list screen
- Quiz attempt screen
- Result/history screen
- API client
- Local storage for caching/history

## Design Choice
This project will start as a monorepo with:
- `backend/` for Python services
- `android/` for the Kotlin Android app

## Future Extensions
- Teacher web dashboard
- LMS integration
- Authentication and roles
- Analytics