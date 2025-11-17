# Times

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

Modern time management and task tracking application built with microservices architecture.

## 🚀 Overview

**Times** is a full-stack application designed to help individuals and teams manage their time effectively, track tasks, and boost productivity. Built with a modular architecture for scalability and maintainability.

## 🏗️ Architecture

This project follows a microservices architecture with separate repositories managed as Git submodules:

```

Times/
├── 📁 backend/ # Core API and business logic
├── 📁 frontend/ # User interface and client-side application
└── 📁 files/ # File storage and asset management service

```

## 📦 Project Structure

| Module       | Description                              | Repository                                                              |
| ------------ | ---------------------------------------- | ----------------------------------------------------------------------- |
| **Backend**  | REST API, database layer, authentication | [Times-backend](https://github.com/Siveruhinthail/Taskly-backend.git)   |
| **Frontend** | Web interface, user dashboard            | [Times-frontend](https://github.com/Siveruhinthail/Taskly-frontend.git) |
| **Files**    | File uploads, storage management         | [Times-files](https://github.com/Siveruhinthail/Taskly-files.git)       |

## 🛠️ Quick Start

### Prerequisites

- Git
- Node.js (version specified in each submodule)
- Docker (optional, for containerized deployment)

### Installation

1. **Clone the main repository with all submodules:**
   ```bash
   git clone --recurse-submodules https://github.com/your-username/Times.git
   cd Times
   ```

````

2. **If you already cloned without submodules:**
   ```bash
   git submodule update --init --recursive
   ```

### Development Setup

Each module has its own development environment. Refer to individual README files in each submodule directory:

- [`backend/README.md`](backend/README.md) - API setup and database configuration
- [`frontend/README.md`](frontend/README.md) - Frontend development server
- [`files/README.md`](files/README.md) - File service configuration

### Running the Application

```bash
# Start backend service
cd backend
npm install
npm run dev

# In new terminal - start frontend
cd frontend
npm install
npm start

# In new terminal - start files service
cd files
npm install
npm run dev
```

## 🔄 Working with Submodules

### Updating Submodules

```bash
# Pull latest changes for all submodules
git submodule update --remote

# Update a specific submodule
git submodule update --remote frontend
```

### Making Changes to Submodules

1. Navigate to the submodule directory:

   ```bash
   cd frontend
   ```

2. Make changes and commit as usual:

   ```bash
   git add .
   git commit -m "Your commit message"
   git push origin main
   ```

3. Update main repository to point to new submodule commit:
   ```bash
   cd ..
   git add frontend
   git commit -m "Update frontend submodule to latest version"
   git push origin main
   ```

## 🌟 Features

- ✅ **Task Management** - Create, organize, and track tasks
- ⏱️ **Time Tracking** - Monitor time spent on activities
- 👥 **Team Collaboration** - Share projects and assign tasks
- 📊 **Analytics** - Productivity insights and reports
- 🔐 **Secure Authentication** - User accounts and permissions
- 📁 **File Attachments** - Attach documents to tasks and projects

## 🚧 Development

### Branch Strategy

- `main` - Production-ready code
- `develop` - Integration branch for features
- `feature/*` - New features and improvements
- `hotfix/*` - Critical production fixes

### Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Support

If you have any questions or need help with setup:

- Open an [Issue](../../issues)
- Check the [Discussions](../../discussions)
- Contact the development team

---

**Built with ❤️ for better time management**

```
````
