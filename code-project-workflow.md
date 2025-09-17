# Code Project Creation Workflow

## Overview
Complete workflow for creating production-ready code projects with proper structure, tooling, and GitHub deployment.

## When to Use
- Starting new development projects
- Creating applications or services
- Building tools or libraries
- Setting up production-ready codebases

## Workflow Steps

### 1. Project Analysis & TodoWrite Setup
```javascript
TodoWrite({
  todos: [
    { content: "Analyze project requirements and tech stack", status: "pending", priority: "high" },
    { content: "Create project directory structure", status: "pending", priority: "high" },
    { content: "Setup configuration files (package.json, etc.)", status: "pending", priority: "high" },
    { content: "Create core implementation files", status: "pending", priority: "high" },
    { content: "Add testing framework and initial tests", status: "pending", priority: "medium" },
    { content: "Create documentation and README", status: "pending", priority: "medium" },
    { content: "Setup GitHub repository and push", status: "pending", priority: "medium" },
    { content: "Verify project can be cloned and run", status: "pending", priority: "high" }
  ]
})
```

### 2. Technology-Specific Structures

#### Frontend (React/Next.js)
```
project-name/
├── src/
│   ├── components/
│   ├── pages/ or app/
│   ├── hooks/
│   ├── utils/
│   └── styles/
├── public/
├── tests/ or __tests__/
├── package.json
├── tsconfig.json (if TypeScript)
├── tailwind.config.js (if Tailwind)
├── .env.example
├── .gitignore
└── README.md
```

#### Backend API (Node.js)
```
project-name/
├── src/
│   ├── routes/
│   ├── models/
│   ├── middleware/
│   ├── services/
│   ├── utils/
│   └── config/
├── tests/
├── package.json
├── .env.example
├── .gitignore
└── README.md
```

#### Python Project
```
project-name/
├── src/ or project_name/
├── tests/
├── requirements.txt or pyproject.toml
├── .env.example
├── .gitignore
├── setup.py (if package)
└── README.md
```

### 3. Essential Configuration Files

#### package.json Template
```json
{
  "name": "project-name",
  "version": "1.0.0",
  "description": "Project description",
  "main": "index.js",
  "scripts": {
    "dev": "development server command",
    "build": "production build command",
    "test": "test runner command",
    "lint": "linting command",
    "start": "production start command"
  },
  "dependencies": {},
  "devDependencies": {}
}
```

#### .env.example Template
```
# Database
DATABASE_URL=your_database_url_here

# API Keys
API_KEY=your_api_key_here

# Environment
NODE_ENV=development
```

### 4. Code Project README Template
```markdown
# Project Name

Brief description of what the project does and its purpose.

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ (or relevant requirements)
- Package manager (npm/yarn/pnpm)
- Any other requirements

### Installation
```bash
git clone https://github.com/username/project-name.git
cd project-name
npm install
cp .env.example .env
# Edit .env with your values
```

### Development
```bash
npm run dev
```

## 🏗️ Project Structure
```
src/
├── components/     # Reusable components
├── pages/         # Application pages
└── utils/         # Utility functions
```

## 🧪 Testing
```bash
npm run test
```

## 📝 API Documentation
Brief API documentation or link to detailed docs

## 🛠️ Built With
- Technology 1
- Technology 2
- Technology 3

## 🤝 Contributing
1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## 📄 License
This project is licensed under the MIT License
```

### 5. Implementation Strategy
1. **Structure First**: Create directories and configuration files
2. **Core Logic**: Implement main functionality
3. **Testing**: Add tests as you build features
4. **Documentation**: Keep README updated throughout
5. **Quality Checks**: Run linting and tests before completion

### 6. Pre-Deployment Quality Checks
```bash
# Run these before considering project complete:
npm run lint          # Code quality
npm run test          # All tests passing  
npm run build         # Production build works
npm start             # Production mode works
```

### 7. GitHub Repository Setup
- Create repository with descriptive name
- Add comprehensive README.md
- Include appropriate .gitignore
- Add LICENSE file
- Set up basic issue templates (optional)

## Technology-Specific Considerations

### React/Next.js Projects
- Include TypeScript configuration
- Add ESLint and Prettier
- Set up testing with Jest/Vitest + Testing Library
- Include CSS framework (Tailwind recommended)
- Add basic components and routing

### Node.js APIs
- Include Express or Fastify setup
- Add CORS, helmet, and security middleware
- Include database connection setup
- Add input validation (Joi/Yup)
- Include API documentation setup (Swagger/OpenAPI)

### Python Projects  
- Include virtual environment setup instructions
- Add requirements.txt or pyproject.toml
- Include pytest configuration
- Add type hints and mypy configuration
- Include basic CLI setup if applicable

## Success Criteria
- ✅ Project follows technology best practices
- ✅ All configuration files are properly set up
- ✅ Core functionality is implemented and working
- ✅ Tests are included and passing
- ✅ Documentation is comprehensive
- ✅ Project can be cloned and run immediately
- ✅ Code quality tools are configured and passing
- ✅ Repository is properly structured on GitHub

## Example Triggers
- "Create a React project"
- "Start a new Node.js API"
- "Build a Python web scraper"
- "Set up a full-stack application"