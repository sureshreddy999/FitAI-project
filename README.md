# FitAI – AI Fitness Assistant 🤖💪

FitAI is an AI-powered fitness web application designed to provide personalized fitness recommendations using Generative AI. The project combines full-stack web development, REST APIs, cloud database integration, and Google's Gemini API to deliver an interactive fitness assistant.

## 🚀 Features

- 🤖 **AI-Powered Recommendations:** Generate personalized fitness recommendations using the Google Gemini API.
- ⚛️ **Interactive Frontend:** User interface built with React.js.
- 🖥️ **Backend Services:** REST API development using Node.js and Express.js.
- 🗄️ **Database Integration:** Amazon DynamoDB for NoSQL data storage.
- ☁️ **Cloud Integration:** AWS services for cloud-based application functionality.
- 🔗 **API Integration:** Communication between frontend, backend, and AI services.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| React.js | Frontend development |
| JavaScript | Application logic |
| Node.js | Backend runtime |
| Express.js | REST API development |
| Google Gemini API | Generative AI integration |
| Amazon DynamoDB | NoSQL database |
| AWS | Cloud services |
| Git & GitHub | Version control |

## 🏗️ System Architecture

```text
                 User
                  |
                  v
           React.js Frontend
                  |
               REST APIs
                  |
                  v
          Node.js / Express.js
             /           \
            v             v
      Gemini API      Amazon DynamoDB
      AI Responses     Data Storage
```

The React frontend communicates with the Node.js and Express.js backend through REST APIs. The backend integrates with the Gemini API to generate AI-powered responses and uses DynamoDB for supported data storage operations.

## 📂 Project Structure

The structure below is illustrative. Update it to match the actual folders in your repository.

```text
FitAI/
├── client/              # React frontend
│   ├── public/
│   ├── src/
│   └── package.json
├── server/              # Node.js backend
│   ├── routes/
│   ├── controllers/
│   ├── services/
│   ├── server.js
│   └── package.json
├── .gitignore
├── .env.example
└── README.md
```

## ⚙️ Prerequisites

Before running the project, ensure you have:

- Node.js and npm installed
- Git installed
- A Google Gemini API key
- An AWS account and appropriate permissions if using DynamoDB

Verify your installations:

```bash
node --version
npm --version
git --version
```

## 🔧 Installation and Setup

### 1. Clone the Repository

Replace the URL with your actual FitAI repository URL.

```bash
git clone https://github.com/sureshreddy999/FitAI.git
cd FitAI
```

### 2. Install Dependencies

If your repository contains separate frontend and backend folders:

```bash
cd client
npm install
```

Open another terminal for the backend:

```bash
cd server
npm install
```

If your repository uses a different folder structure, run `npm install` in the directory containing the appropriate `package.json`.

### 3. Configure Environment Variables

Create a `.env` file in the appropriate backend directory.

Example configuration:

```env
PORT=5000
GEMINI_API_KEY=your_gemini_api_key
AWS_REGION=your_aws_region
DYNAMODB_TABLE_NAME=your_dynamodb_table
```

These are example variable names. Match them to the variables expected by your code.

**Security:** Never commit API keys, AWS credentials, passwords, or other secrets to GitHub. Add `.env` to `.gitignore` and use secure environment-variable or secrets-management practices.

### 4. Configure AWS DynamoDB

If your application uses DynamoDB:

1. Create the required DynamoDB table.
2. Configure the correct AWS region.
3. Set up AWS authentication securely.
4. Grant the application only the permissions it needs.
5. Ensure the table name and schema match your backend implementation.

### 5. Start the Backend

Run the command supported by your backend's `package.json`. For example:

```bash
npm start
```

For development, your project may support:

```bash
npm run dev
```

### 6. Start the Frontend

In the frontend terminal, run the command supported by your project.

For a React application using a standard npm start script:

```bash
npm start
```

For a Vite-based application:

```bash
npm run dev
```

Open the local URL displayed in the terminal.

## 🔑 AI Integration

FitAI integrates Google's Gemini API for AI-powered fitness recommendations.

The typical request flow is:

1. The user provides fitness-related input.
2. The frontend sends the request to the backend.
3. The backend validates the input and prepares the AI request.
4. The backend communicates with the Gemini API.
5. The generated response is returned to the frontend.

Keep the Gemini API key on the server side. Do not expose it in browser code.

## 🗄️ Database Integration

Amazon DynamoDB is used for NoSQL database functionality.

Depending on the implementation, the backend can use database operations to store or retrieve relevant application data. Ensure database permissions and error handling are configured appropriately.

## 🧪 Testing

Recommended areas to test include:

- Frontend rendering and user interactions
- REST API request and response handling
- Input validation and error handling
- Gemini API failures and unexpected responses
- DynamoDB operations
- Missing environment variables
- Backend and frontend integration

Run automated tests if they are configured in the project.

## 🔒 Security Considerations

- Store secrets outside the source code.
- Validate incoming API requests.
- Configure CORS appropriately.
- Use least-privilege AWS permissions.
- Avoid logging sensitive information.
- Treat AI-generated fitness recommendations as general information, not medical advice.

## 🔮 Future Enhancements

Potential future improvements include:

- User authentication and personalized profiles
- Workout planning and progress tracking
- Nutrition tracking
- Enhanced recommendation personalization
- Automated testing and CI/CD
- Cloud deployment and monitoring
- Improved error handling and application observability

These are possible enhancements, not claims about currently implemented features.

## 👨‍💻 Author

**Suresh Reddy Dwarampudi**

- GitHub: [sureshreddy999](https://github.com/sureshreddy999)
- LinkedIn: [Suresh Reddy Dwarampudi](https://www.linkedin.com/in/suresh-reddy-dwarampudi-29b234258/)

## 🤝 Contributing

Contributions and suggestions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Make your changes.
4. Test your changes.
5. Submit a pull request.


---

⭐ If you find this project interesting, consider starring the repository!
