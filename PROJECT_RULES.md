# AgroVision AI Project Rules

## Project Goal

Build an Intelligent Crop Disease Identification System that allows a user to upload a crop/leaf image and receive AI-assisted disease identification, confidence information, disease explanation, severity information and agricultural guidance.

The system must clearly communicate that AI predictions are advisory and should not be treated as definitive agricultural or medical/laboratory diagnosis.

## Technology

Frontend:
React + Vite + Tailwind CSS

Backend:
Python + FastAPI

Machine Learning:
PyTorch

Database:
Supabase/PostgreSQL

Storage:
Supabase Storage

AI Assistant:
LLM-based agricultural assistant with appropriate retrieval/context.

## Repository Responsibilities

Backend/
- FastAPI application
- API routes
- ML inference integration
- backend services

ML/
- dataset preparation
- preprocessing
- training
- evaluation
- inference
- explainability

frontend/
- React application
- UI
- dashboard
- image upload
- prediction results
- history
- assistant interface

Database/
- database schema
- migrations/schema documentation
- seed data
- database-related configuration

## Collaboration Rules

1. main must remain stable.
2. Never develop features directly on main.
3. Each developer works on their own feature branch.
4. Pull the latest main before starting major work.
5. Make small commits.
6. Do not modify unrelated files.
7. Do not overwrite another developer's work.
8. Use Pull Requests before merging feature work into main.
9. Test changes before creating a Pull Request.

## AI Coding Rules

1. Inspect the existing repository before changing files.
2. Make small controlled changes.
3. Do not rewrite working code unnecessarily.
4. Do not modify another developer's assigned area.
5. Report all files changed.
6. Test changes after implementation.
7. Never commit API keys or passwords.
8. Never fabricate ML performance.
9. Never fabricate agricultural facts.
10. Do not install unnecessary dependencies.

## ML Rules

1. Keep training and inference logically separated.
2. Prevent data leakage.
3. Track dataset versions/source.
4. Evaluate using accuracy, precision, recall and F1-score.
5. Generate a confusion matrix.
6. Record limitations of the dataset.
7. Do not claim laboratory-level accuracy.
8. The model should return confidence information.
9. Explainability should be included where technically appropriate.

## Backend Rules

1. Use FastAPI.
2. Keep API routes separate from ML logic.
3. Validate inputs.
4. Use consistent JSON responses.
5. Handle errors properly.
6. Never hardcode secrets.

## Frontend Rules

1. Use reusable React components.
2. Keep API calls in a service layer.
3. Implement loading states.
4. Implement error states.
5. Keep the UI responsive.
6. Do not hardcode production API responses.

## Security

Never commit:
- API keys
- passwords
- database credentials
- private tokens
- .env files

## Data Safety

Use legitimate agricultural datasets with appropriate licensing.

Clearly distinguish:
- model prediction
- confidence
- agricultural information
- user-provided information
