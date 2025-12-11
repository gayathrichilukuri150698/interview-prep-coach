# Interview Prep Coach 🤖

An AI-powered chatbot designed to help people prepare for tech interviews. Get personalized practice questions, mock interview simulations, and detailed feedback for coding, system design, and behavioral interviews.

## Features

- 💻 **Coding Questions**: Practice algorithms and data structures with personalized difficulty
- 🏗️ **System Design**: Learn to design scalable systems with expert feedback
- 💬 **Behavioral Questions**: Master the STAR method for behavioral interviews
- 🎯 **Mock Interviews**: Simulate real interview scenarios with AI feedback
- ⚙️ **Personalized**: Customize your profile based on role, experience level, and focus areas
- 🎨 **Beautiful UI**: Modern, responsive interface built with Next.js and Tailwind CSS

## Getting Started

### Prerequisites

- Node.js 18+ installed
- OpenAI API key ([Get one here](https://platform.openai.com/api-keys))

### Installation

1. **Clone or navigate to the project directory:**
   ```bash
   cd interview-prep-coach
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Set up environment variables:**
   ```bash
   cp .env.example .env
   ```
   
   Then edit `.env` and add your OpenAI API key:
   ```
   OPENAI_API_KEY=your_openai_api_key_here
   ```

4. **Run the development server:**
   ```bash
   npm run dev
   ```

5. **Open your browser:**
   Navigate to [http://localhost:3000](http://localhost:3000)

## Usage

1. **Set Your Profile**: Click the settings icon to configure your role, experience level, and focus areas
2. **Choose Mode**: 
   - **Practice Mode**: Get questions and explanations at your own pace
   - **Mock Interview Mode**: Simulate a real interview with one question at a time
3. **Start Practicing**: 
   - Use quick action buttons for common requests
   - Type your questions or responses
   - Get AI-powered feedback and guidance

## Project Structure

```
interview-prep-coach/
├── app/
│   ├── api/
│   │   └── chat/          # API route for OpenAI integration
│   ├── globals.css         # Global styles
│   ├── layout.tsx          # Root layout
│   └── page.tsx            # Main chat interface
├── components/
│   ├── ChatMessage.tsx     # Message component
│   ├── InterviewModeSelector.tsx  # Mode switcher
│   └── UserProfileModal.tsx      # Profile settings
├── package.json
└── README.md
```

## Technologies

- **Next.js 14**: React framework with App Router
- **TypeScript**: Type-safe development
- **Tailwind CSS**: Utility-first styling
- **OpenAI API**: GPT-4 for intelligent responses
- **Lucide React**: Beautiful icons

## Customization

### Adjusting Difficulty
The chatbot automatically adapts to your experience level. Update your profile in settings to change difficulty.

### Adding Custom Roles
Edit `components/UserProfileModal.tsx` to add more role options.

### Modifying System Prompts
The system prompt is generated in `app/page.tsx` in the `generateSystemPrompt` function. Customize it to change the chatbot's behavior.

## Troubleshooting

**Error: "OpenAI API key not configured"**
- Make sure you've created a `.env` file with your `OPENAI_API_KEY`

**Error: "Invalid API key"**
- Verify your API key is correct and has sufficient credits

**Build errors**
- Run `npm install` again to ensure all dependencies are installed
- Check that you're using Node.js 18+

## License

MIT License - feel free to use this project for your interview preparation!

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

---

**Happy Interview Prep! 🚀**

