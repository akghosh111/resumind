# 🚀 Resume Analyzer & Feedback App 📝

This project is a React-based application designed to help users analyze and improve their resumes. It allows users to upload their resume (in PDF format), convert it to an image, and then leverages AI to provide detailed feedback on various aspects, such as ATS compatibility, content quality, structure, and skills. The application provides a user-friendly interface for reviewing the resume and the AI-generated feedback, empowering users to create more effective resumes.

## ✨ Key Features

- **Resume Upload:** Users can easily upload their resumes in PDF format.
- **PDF to Image Conversion:** The application automatically converts the uploaded PDF into an image for easy viewing.
- **AI-Powered Analysis:** Leverages AI to provide comprehensive feedback on resume quality.
- **ATS Compatibility Score:**  Provides a score indicating how well the resume is likely to perform in Applicant Tracking Systems.
- **Detailed Feedback:** Offers insights into tone and style, content, structure, and skills.
- **Actionable Suggestions:** Provides specific suggestions for improving the resume based on the AI analysis.
- **User Authentication:** Secure authentication to protect user data and ensure privacy.
- **Resume Storage:** Securely stores uploaded resumes and associated data.
- **Dynamic Routing:** Uses `@react-router/dev` for efficient and flexible navigation.

## 🛠️ Tech Stack

| Category      | Technology                                  | Description                                                                                                |
|---------------|---------------------------------------------|------------------------------------------------------------------------------------------------------------|
| Frontend      | React                                       | JavaScript library for building user interfaces.                                                           |
| Routing       | @react-router/dev                           | Routing library for React applications, enabling server-side rendering (SSR).                               |
| State Management| Zustand                                       | A small, fast and scalable bearbones state-management solution.                                           |
| UI Components | Custom React Components                     | Reusable components for UI elements like file uploaders, score displays, and feedback sections.             |
| Styling       | Tailwind CSS                                | A utility-first CSS framework for rapidly building custom designs.                                         |
| PDF Rendering | pdfjs-dist                                  | PDF.js library for rendering PDF documents in the browser.                                                |
| AI            | (External AI Service via `window.puter.ai`) | An external AI service (likely accessed through an API) for analyzing resumes and generating feedback.     |
| Storage       | (External Storage via `window.puter.fs`)    | An external file storage service (likely accessed through an API) for storing uploaded resumes and images. |
| Key-Value Store| (External KV Store via `window.puter.kv`)   | An external key-value store (likely accessed through an API) for storing resume metadata and feedback.    |
| Utilities     | clsx, tailwind-merge                        | Utilities for class name manipulation and Tailwind CSS conflict resolution.                                 |
| Build Tools   | Vite       | Bundler and build tool for the React application.                                                          |
| Language      | TypeScript                                  | Provides static typing for enhanced code quality and maintainability.                                     |

## 📦 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- A `window.puter` service (likely requires an account and setup)

### Installation

1.  Clone the repository:

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2.  Install dependencies:

    ```bash
    npm install # or yarn install
    ```

3.  Configure Environment Variables:

    *   This project relies on a `window.puter` object, which is assumed to be provided by an external service. Ensure that this service is properly initialized and configured in your environment.  Specific configuration steps will depend on the `window.puter` service being used.

### Running Locally

1.  Start the development server:

    ```bash
    npm run dev # or yarn dev
    ```

2.  Open your browser and navigate to `http://localhost:<port>` (usually port 3000 or similar).

## 📂 Project Structure

```
├── app
│   ├── components
│   │   ├── ATS.tsx             # Component for displaying ATS score and suggestions
│   │   ├── FileUploader.tsx    # Reusable file uploader component
│   │   ├── Navbar.tsx          # Navigation bar component
│   │   ├── ResumeCard.tsx      # Component for displaying a resume card
│   │   ├── ScoreBadge.tsx      # Component for displaying a score badge (assumed)
│   │   ├── ScoreGauge.tsx      # Component for displaying a score gauge (assumed)
│   │   ├── Summary.tsx         # Component for displaying resume feedback summary
│   │   └── Details.tsx         # Component for displaying detailed resume analysis results (assumed)
│   ├── lib
│   │   ├── pdf2image.ts        # Utility function to convert PDF to image
│   │   ├── puter.ts            # Zustand store and types for interacting with window.puter
│   │   └── utils.ts            # Utility functions (cn, formatSize, generateUUID)
│   ├── routes
│   │   ├── auth.tsx            # Authentication route
│   │   ├── home.tsx            # Home page route
│   │   ├── resume.tsx          # Resume review route
│   │   └── upload.tsx          # Upload route
│   ├── +types
│   │   ├── home.ts             # Type definitions for the home component
│   │   └── root.ts             # Type definitions for the root component
│   ├── app.css               # Main application stylesheet
│   ├── root.tsx              # Root component of the application
│   └── routes.ts             # Defines the routes for the application
├── constants
│   └── index.ts            # Constant data (resumes array, AI response format)
├── public
│   └── pdf.worker.min.mjs  # PDF.js worker file
├── types
│   └── index.d.ts          # TypeScript interface definitions
├── react-router.config.ts  # Configuration for @react-router/dev
├── package.json
├── tsconfig.json
└── README.md
```

## 📸 Screenshots

To be added soon ...

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Make your changes and commit them with clear and concise messages.
4.  Submit a pull request.

## 📝 License

This project is licensed under the [MIT License](LICENSE).

## 📬 Contact

For questions or inquiries, please contact: [Your Name/Organization] at [Your Email/Website]

## 💖 Thanks

Thank you for checking out this project! We hope it helps you improve your resume and land your dream job.


