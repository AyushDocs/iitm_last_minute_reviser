<!-- @format -->

# StudyAI - Intelligent Learning Assistant 🎓

StudyAI transforms your course content into personalized learning materials using artificial intelligence. Convert videos, lecture slides, and notes into interactive flashcards, summaries, and practice questions.

## 🌟 Features

### Content Processing

-   📺 YouTube video transcription and analysis
-   📄 PDF and document parsing (lecture slides, notes)
-   📝 Text extraction and processing
-   📊 Automatic content organization

### AI-Powered Learning Tools

-   🔍 Smart summarization of complex topics
-   💡 Key concept extraction
-   🎴 Automated flashcard generation
-   ❓ Practice question creation
-   📚 Topic clustering and relationship mapping

### User Features

-   📋 Customizable study plans
-   📈 Progress tracking
-   🔎 Advanced search capabilities
-   💾 Export options for created content
-   🎯 Spaced repetition learning system

## 🛠️ Tech Stack

### Backend

-   **Python** (3.9+)
    -   FastAPI
    -   Langchain
    -   Transformers (Hugging Face)
    -   OpenAI Integration
    -   youtube-dl
    -   PyPDF2

### Frontend

-   **React.js/Next.js**
    -   Material UI
    -   React Query
    -   Redux (optional)

### Database

-   PostgreSQL
-   MongoDB
-   Redis (caching)

### Storage

-   AWS S3

## 🚀 Getting Started

### Prerequisites

-   Python 3.9+
-   Node.js 16+
-   PostgreSQL
-   MongoDB
-   Redis

### Installation

1. Clone the repository

git clone https://github.com/yourusername/studyai.git

cd studyai

2. Set up backend

```bash
# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
```

3. Set up frontend

```bash
cd frontend
npm install
```

4. Start the application

```bash
# Start backend
python run.py

# Start frontend (new terminal)
cd frontend
npm run dev
```

## 🔧 Configuration

Create a `.env` file in the root directory:

```
# API Keys
OPENAI_API_KEY=your_openai_key
AWS_ACCESS_KEY=your_aws_key
AWS_SECRET_KEY=your_aws_secret

# Database
DATABASE_URL=postgresql://user:password@localhost:5432/studyai
MONGODB_URI=mongodb://localhost:27017/studyai
REDIS_URL=redis://localhost:6379

# Application
DEBUG=True
SECRET_KEY=your_secret_key
```

## 📁 Project Structure

```
studyai/
├── backend/
│   ├── api/
│   ├── core/
│   ├── processors/
│   ├── models/
│   └── services/
├── frontend/
│   ├── components/
│   ├── pages/
│   ├── styles/
│   └── utils/
├── tests/
└── docs/
```

## 🔄 API Endpoints

### Content Processing

-   `POST /api/v1/content/process` - Process new content
-   `GET /api/v1/content/{id}` - Retrieve processed content
-   `POST /api/v1/ai/generate` - Generate learning materials

### User Management

-   `POST /api/v1/auth/register` - Register new user
-   `POST /api/v1/auth/login` - User login
-   `GET /api/v1/user/progress` - Get learning progress

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📜 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## 🙏 Acknowledgments

-   OpenAI for GPT models
-   Hugging Face for transformer models
-   All contributors and supporters

## 📞 Contact

Your Name - [@yourtwitter](https://twitter.com/yourtwitter) - email@example.com

Project Link: [https://github.com/yourusername/studyai](https://github.com/yourusername/studyai)

---

⭐️ If you find this project helpful, please give it a star!


