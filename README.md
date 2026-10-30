# PROJECT FORGE — CodeMind

A college-demo full-stack MVP:
- React + TypeScript + Vite frontend
- Java Spring Boot REST backend
- H2 file database (no PostgreSQL required)
- Project create/list/delete
- Code analysis for Java, Python, JavaScript, TypeScript using practical rule-based checks
- Analysis history and summary statistics
- Team image preview/upload in the browser (preview only; see note below)

## Requirements
- JDK 17+ (your JDK 25 should work with Spring Boot 3.4.5, but verify locally)
- Node.js 20+ and npm
- Internet for first Maven/npm dependency downloads

## Run backend (Windows CMD)
```cmd
cd /d "%USERPROFILE%\Downloads\PROJECT_FORGE_REBUILT\backend"
"%USERPROFILE%\Downloads\apache-maven-3.10.0-bin\apache-maven-3.10.0\bin\mvn.cmd" spring-boot:run
```
Backend: http://localhost:8080
Health: http://localhost:8080/api/health

## Run frontend (second CMD window)
```cmd
cd /d "%USERPROFILE%\Downloads\PROJECT_FORGE_REBUILT\frontend"
npm install
npm run dev
```
Open the URL Vite prints (normally http://localhost:5173).

## Important verification note
This archive is generated as a practical starter, but it has not been compiled or run in your local Windows environment here. Run the commands above and share any exact error output so it can be fixed.

## CodeMind scope
Analysis is rule-based static checking, not a hosted LLM/AI service. It catches common patterns and returns file/line/severity findings. It is intended for a college demo, not as a replacement for a compiler, linter, or security scanner.

## Team image
The image picker currently previews a selected image in the frontend only. Persistent server-side image storage can be added later.
