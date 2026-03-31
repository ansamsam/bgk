# Product Requirements Document (PRD): pusulam MVP

## 1. Project Goal & Philosophy
**Goal:** Create a minimalist, mobile-friendly web SITE that uses Gemini AI to help working children pass Open High School (AÖL) exams by focusing on the most critical content. Contain content from the1st grade to the 12th.
**Philosophy:** "Time is the greatest treasure." Optimize study time by 70% by focusing on the strategic 20% of the curriculum that yields 80% of exam results.

## 2. Tech Stack & Implementation Roadmap
- **Frontend:** React.js / Next.js (Tailwind CSS for styling).
- **AI:** Google Gemini API (via Google AI Studio).
- **Backend/DB:** Supabase (Auth, Chat, Storage for Audio/PDF).
- **Deployment:** Lovable / Vercel.

### Development Tasks:
- **Task 1: Core UI Construction** -> Create a clean structure with subject/grade inputs and a "Generate Study Plan" button.
- **Task 2: AI Integration** -> Connect Gemini API to process curriculum data and generate summaries/questions.
- **Task 3: Business Logic** -> Handle API calls to return "Contextual Summaries" and "Kritik 20" question sets.
- **Task 4: Mobile-First Design** -> Finalize Tailwind UI with high contrast (Dark Mode) for industrial environments.
- **Task 5: PWA & Deployment** -> Enable offline caching and deploy to Lovable/Vercel.

## 3. Detailed Feature Modules

### Module A: Strategic Navigation (AI Driven)
- **Input:** Grade (e.g., 10th Grade) and Subject (e.g., Math 1).
- **Visual Heatmap:** Color-coded subjects by exam frequency (Red: Essential, Yellow: Recommended).
- **Exam Countdown:** Days remaining vs. completion percentage of critical topics.
- **AI Output:** "Must-Know" bullet points and a "Kritik 20" list containing the most frequent past exam types.

### Module B: Contextual Learning (Applied Theory)
- **Sector Adaptation:** Users select their work sector (Sanayi, Tekstil, Satış).
- **Applied Metaphors:** AI explains topics using workplace tools (e.g., "Explain Physics Levers using a car jack").
- **Audio Recaps:** Text-to-speech functionality for 10-minute "Podcast-style" lesson summaries.

### Module C: Exam Rescue Pack (Kritik 20)
- **PDF/List Generator:** Dynamically creates a 20-question set based on past MEB exam analysis.
- **Interactive Solutions:** QR codes or links leading to mentor-prepared solution notes or videos.
- **Success Tracker:** A checkbox system to mark "Mastered" for each of the 20 question types.

### Module D: Secure Mentor Bridge (Buddy System)
- **Safe Chat:** Simple text-based chat with image upload for quick question solving.
- **Status Management:** User/Mentor status toggles (e.g., "At work", "Studying", "Available").
- **STK Oversight:** Admin panel to verify mentors and monitor interactions for safety.

## 4. UI/UX & Accessibility Requirements
- **Minimalist Dashboard:** No complex menus. Direct prompt: "Which subject will you study for 10 minutes?"
- **Focus Mode:** A "I have 15 minutes" button that shows only 3 high-priority flashcards.
- **Accessibility:** Large buttons and high-contrast fonts for low-light factory/workshop conditions.
- **Offline Mode (PWA):** Cache "Kritik 20" and audio summaries for use without internet.

## 5. User Flows
1. **Onboarding:** User selects "Job Sector" and "Target Exam".
2. **Solving:** User solves 5 "Hot Questions" during a break.
3. **Asking:** User uploads a photo of a hard question; Mentor receives a notification via the STK-managed bridge.

## 6. Security & Data Privacy
- **Verification:** Only STK-approved mentors get the "Verified" badge.
- **Privacy:** Minimal data collection; no home addresses or sensitive employer details.
- **Environment Variables:** Secure handling of API keys in Lovable/Vercel.  # Tech Stack: Yol Arkadaşım (Study Buddy) 🛠️

The project is designed to be a high-velocity MVP that is scalable, cost-effective, and mobile-first.

## Frontend (User Interface)
- **Framework:** Next.js (React) -> For SEO optimization and native-like PWA support.
- **Styling:** Tailwind CSS -> For rapid, mobile-first UI development.
- **State Management:** Zustand or React Context API -> For lightweight and efficient client-side state handling.
- **PWA Features:** `next-pwa` -> To enable offline access and "Add to Home Screen" functionality for workers with unstable internet.

## Backend & Database (Infrastructure)
- **Platform:** Supabase (Backend-as-a-Service)
    - **PostgreSQL:** To store user profiles, grade levels, and lesson progress.
    - **Authentication:** Secure login via Email and Phone (OTP).
    - **Real-time:** WebSockets for instant Mentor-Student messaging.
    - **Storage:** S3-compatible buckets for audio lesson summaries (MP3) and question images.

## Artificial Intelligence (Intelligence Layer)
- **Engine:** Google Gemini 1.5 Flash (via Google AI Studio)
    - **Core Tasks:** Curriculum analysis, contextual theory generation (e.g., car jack physics examples), and generating scripts for audio summaries.
- **Text-to-Speech (TTS):** Web Speech API or Google Cloud TTS -> To convert AI-generated summaries into listenable content.

## Deployment & DevOps
- **Hosting:** Vercel -> Seamless integration with the Next.js ecosystem.
- **CI/CD:** GitHub Actions -> Automated testing and deployment pipelines.
- **Monitoring:** Sentry -> Real-time error tracking and performance monitoring.

## Security & Safety
- **Content Filtering:** Gemini API safety settings to ensure child-safe educational content.
- **Environment Variables:** Protection of sensitive API keys and secrets via `.env` management. # User Flow: Study Buddy
