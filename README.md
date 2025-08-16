# Full-Stack-AI-Mock-Interview-Web-Application
Built an AI-powered full-stack web app for mock interviews, featuring live AI avatar interviews, automated real-time feedback, and secure subscription management.

Description:
• Developed a comprehensive full-stack AI mock interview application completely from scratch, designed to provide AI-powered practice sessions for mastering job interviews.
• The application features a live streaming AI avatar that conducts mock interviews and provides real-time feedback.
Key Features & Accomplishments:
• AI-Driven Interview Generation:
    ◦ Engineered a system to generate AI mock interview questions based on user-uploaded resumes or inputted job descriptions and titles.
    ◦ Orchestrated complex application workflows using n8n automation, allowing for efficient, drag-and-drop logic for AI question generation and feedback.
    ◦ Integrated ImageKit for free cloud storage of uploaded PDF resumes, facilitating content extraction for AI processing.
    ◦ Utilized OpenAI's ChatGPT (or other AI models like Gemini) to power question generation based on provided resume/job data and to analyze conversations for feedback.
• Interactive Interview Experience:
    ◦ Integrated Akul's streaming avatar API to connect users to a live AI agent for mock interviews, enabling real-time listening and interaction.
    ◦ Displayed live conversation transcripts during the interview session.
    ◦ Provided intuitive in-call controls including mute/unmute and call termination.
• Automated Feedback & Reporting:
    ◦ Implemented a system to generate detailed interview feedback (including suggestions and a rating out of 10) within seconds after an interview concludes.
    ◦ Processed interview conversation messages through n8n's AI workflow to produce this comprehensive feedback.
• Robust User Management & Security:
    ◦ Integrated Clerk for comprehensive and secure authentication, supporting Gmail, email/password, and social sign-on methods.
    ◦ Utilized Clerk's subscription billing feature to implement free and paid membership tiers (e.g., limiting free users to two interviews daily), easily adding a pricing table and managing payments.
    ◦ Enhanced application security and implemented rate limiting for interview creation, bot detection, email validation, and attack protection using Arja.
• Scalable Data Infrastructure:
    ◦ Leveraged Convex as a real-time, open-source database for storing all interview sessions, user information, and application data, benefiting from its type safety, file storage, and serverless functions.
    ◦ Designed database schemas for user profiles and interview sessions, ensuring efficient data retrieval and relationships.
• Modern Web Development Practices:
    ◦ Developed the application using React and Next.js, utilizing Next.js features like folder-based routing, built-in optimization, React Server Components, and client-side rendering for a performant application.
    ◦ Styled the user interface with Tailwind CSS, complemented by ShadCN and Aceternity UI for pre-built, customizable UI components.
    ◦ Managed global application state effectively using React's Context API.
    ◦ Ensured code quality and type safety throughout the development process with TypeScript.
• Deployment & Production Readiness:
    ◦ Successfully deployed the full-stack application to Vercel, enabling continuous integration and delivery.
    ◦ Configured n8n automation workflows for both local development and production environments, with a focus on seamless deployment via Hostinger for scalable AI automation
