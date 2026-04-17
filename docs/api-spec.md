# API Spec Draft

## POST /uploads
Upload a slide file (PDF/PPT)

## POST /jobs/{jobId}/process
Start concept extraction and quiz generation

## GET /jobs/{jobId}
Check processing status

## GET /quizzes/{quizId}
Get generated quiz data

## POST /quizzes/{quizId}/attempt
Submit quiz answers

## GET /students/{studentId}/history
Get quiz attempt history

## Response Shape Example

```json
{
  "quizId": "quiz-001",
  "title": "Intro to Thermodynamics",
  "concepts": [
    "enthalpy",
    "entropy",
    "closed system"
  ],
  "questions": [
    {
      "id": "q1",
      "type": "mcq",
      "question": "Which property measures disorder in a system?",
      "options": ["Enthalpy", "Entropy", "Pressure", "Volume"],
      "answer": "Entropy"
    }
  ]
}