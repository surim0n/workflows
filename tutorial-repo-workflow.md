# Tutorial Repository Creation Workflow

## Overview
Complete workflow for creating educational/course material repositories with comprehensive documentation and GitHub deployment.

## When to Use
- Creating tutorial repositories for courses
- Sharing educational content with students
- Building documentation-heavy projects
- Course material that needs immediate usability

## Workflow Steps

### 1. Initial TodoWrite Setup
```javascript
TodoWrite({
  todos: [
    { content: "Create main content file", status: "pending", priority: "high" },
    { content: "Create comprehensive README.md", status: "pending", priority: "high" },
    { content: "Initialize git repository", status: "pending", priority: "medium" },
    { content: "Commit files to repository", status: "pending", priority: "medium" },
    { content: "Create GitHub repository and push", status: "pending", priority: "high" }
  ]
})
```

### 2. Content Creation Pattern

#### Main Content File Structure
- **Filename**: `[descriptive-name]-prompt.md` or `[topic-name].md`
- **Content**: Core educational material, prompts, or instructions
- **Format**: Clear, well-structured markdown with examples

#### README.md Template
```markdown
# Project Title 🚀

Brief description of the educational content

## 📋 Overview
What this tutorial/tool teaches or provides

## 🚀 Quick Start
1. Clone the repository
2. Follow usage instructions
3. Apply to your specific use case

## 📖 How to Use
Detailed step-by-step instructions

## 🔍 What You'll Learn/Get
- Key learning outcomes
- Tools or knowledge provided
- Expected results

## 📊 Example Output
Sample results, screenshots, or outcomes

## 🛠️ Prerequisites
- Required knowledge
- Tools needed
- Account requirements

## 💡 Best Practices
Tips for getting the best results

## 🤝 Contributing
How others can improve the tutorial

## 📚 Resources
Additional links and references

## 📄 License
MIT License (or appropriate)
```

### 3. File Structure
```
tutorial-name/
├── README.md                    # Comprehensive usage guide
├── main-content.md             # Core tutorial/prompt content
└── (additional files if needed)
```

### 4. Quality Standards
- **Immediate Usability**: Repository should be usable right after cloning
- **Clear Instructions**: No ambiguity in setup or usage
- **Examples Included**: Concrete examples for all concepts
- **Educational Focus**: Optimized for learning and teaching

### 5. GitHub Deployment
```bash
# If git init fails, use GitHub CLI API:
gh api repos/username/repo-name/contents/filename.md -X PUT \
  --field message="Add [description]" \
  --field content="$(base64 < filename.md)"
```

### 6. Success Checklist
- ✅ Repository created and public
- ✅ README is comprehensive and user-friendly
- ✅ Main content is educational and actionable
- ✅ Can be used immediately without additional setup
- ✅ Clear value proposition for learners

## Example Triggers
- "Create a tutorial repo"
- "I need to upload a repo for my course"
- "Make educational content for students"
- "Share a prompt/tool with documentation"

## Key Principles
- **Education First**: Focus on teaching and learning
- **Documentation Heavy**: Comprehensive guides over code
- **Immediate Value**: Usable without complex setup
- **Accessibility**: Clear for all skill levels