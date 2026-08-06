
## Overview

This project is a sophisticated job interview application designed to streamline the interview process using modern web technologies and AI. It generates role-specific interview questions, records candidate responses, and provides AI-driven feedback. The application leverages Gemini AI for analysis and feedback, ensuring candidates receive constructive evaluations based on their performance.

## Features

- **Dynamic Question Generation**: Generates interview questions tailored to the user's job role, job description, and experience.
- **Voice Recording**: Allows users to answer questions via microphone, capturing their responses in real-time.
- **AI-Powered Feedback**: Uses Gemini AI to analyze responses and provide detailed feedback.
- **User Authentication**: Utilizes Clerk for secure user authentication and session management.

## Technologies Used

- **Next.js**: Framework for building the front-end application.
- **PostgreSQL**: Database for storing user data, interview questions, and responses.
- **Drizzle**: ORM (Object-Relational Mapping) to interact with the PostgreSQL database.
- **Neon**: Serverless PostgreSQL with performance optimizations.
- **shadcn/ui**: UI component library for building a responsive and accessible user interface.
- **Clerk**: Authentication service for handling user sign-up, login, and management.
- **Gemini AI**: AI service for analyzing audio responses and providing feedback.
- **Audio Transcript**: Service for transcribing audio responses into text for further processing.

## Installation

### Prerequisites

- Node.js (>= 14.x)
- PostgreSQL
- Yarn or npm
- Clerk API keys
- Gemini AI API keys

### Steps

1. **Clone the Repository**


2. **Install Dependencies**
   ```bash
   yarn install
   # or
   npm install
   ```

3. **Set Up Environment Variables**

   Create a `.env` file in the root directory and add the following variables:
   ```env
   NEXT_PUBLIC_CLERK_FRONTEND_API=your_clerk_frontend_api
   CLERK_API_KEY=your_clerk_api_key
   DATABASE_URL=your_database_url
   GEMINI_API_KEY=your_gemini_api_key
   ```

4. **Run Database Migrations**
   ```bash
   yarn drizzle db:migrate
   # or
   npm run drizzle db:migrate
   ```

5. **Start the Development Server**
   ```bash
   yarn dev
   # or
   npm run dev
   ```

## Usage

1. **Sign Up/Login**: Users need to sign up or log in using Clerk authentication.
2. **Job Role and Description**: Enter job role, job description, and experience details.
3. **Start Interview**: The system generates relevant questions.
4. **Answer Questions**: Users answer questions via microphone.
5. **Receive Feedback**: Gemini AI analyzes responses and provides feedback.



