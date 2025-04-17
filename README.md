# JSW Site Visit Data Chatbot

A chatbot application for querying site visit data using Next.js, Node.js/Express, and Gemini AI.

## Features

- Modern, clean UI similar to popular chat applications
- Real-time chat interface
- Chat history sidebar
- Integration with Gemini API (simulated in demo)
- Responsive design

## Tech Stack

### Frontend
- Next.js 14
- TypeScript
- Tailwind CSS
- Axios for API calls
- React Icons

### Backend
- Node.js
- Express
- TypeScript
- Cors for cross-origin support
- Body-parser for request parsing

## Getting Started

### Prerequisites

- Node.js (v18 or later)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd jsw-site-visit-chatbot
```

2. Install frontend dependencies:
```bash
npm install
```

3. Install backend dependencies:
```bash
cd server
npm install
cd ..
```

### Environment Setup

1. Create `.env.local` in the root directory for the frontend:
```
NEXT_PUBLIC_API_URL=http://localhost:5000/api
```

2. Create `.env` in the server directory for the backend:
```
PORT=5000
NODE_ENV=development
# Add Gemini API key when integrating with the actual Gemini API
# GEMINI_API_KEY=your_api_key
```

### Running the Application

1. Start the backend server:
```bash
cd server
npm run dev
```

2. In a separate terminal, start the frontend:
```bash
# From the root directory
npm run dev
```

3. Open your browser and navigate to `http://localhost:3000`

## How It Works

- The frontend sends user messages to the backend API
- The backend processes the messages (using Gemini AI in production)
- Responses are sent back to the frontend and displayed in the chat interface
- Chat history is maintained on both client and server side

## Future Enhancements

- Integration with actual Gemini API
- User authentication
- More advanced data querying capabilities
- Export chat history
- Voice input support

## License

This project is licensed under the MIT License - see the LICENSE file for details.
