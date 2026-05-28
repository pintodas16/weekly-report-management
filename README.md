# 📋 Weekly Report Management

[![Angular](https://img.shields.io/badge/Angular-17%2B-red?style=flat-square&logo=angular)](https://angular.io/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.3-3178c6?style=flat-square&logo=typescript)](https://www.typescriptlang.org/)
[![NG-ZORRO](https://img.shields.io/badge/NG--ZORRO-UI%20Components-blue?style=flat-square)](https://ng.ant.design/)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)

> A modern, intuitive Angular application for managing weekly team reports and individual task tracking. Designed for agile teams seeking a lightweight, no-backend solution to maintain visibility over team members, their progress, and blockers.

## 🌐 Live Demo

**[https://weekly-report-management.vercel.app/](https://weekly-report-management.vercel.app/)**

---

## ✨ Features

- **👥 Team Management**
  - Add and manage team members with assigned roles (e.g., Developer, Manager, Team Lead)
  - Flexible role customization for various team structures

- **✅ Task Tracking**
  - Create tasks per team member with detailed information:
    - Module name
    - Task description
    - Priority levels (Low, Medium, High)
    - Progress tracking with interactive slider (0-100%)
    - Blocker descriptions and notes
  - Weekly tracking with editable task drawers for quick updates

- **💾 Data Persistence**
  - LocalStorage-based persistence — no backend required
  - All data stored locally for instant access and offline capability

- **🎨 User Experience**
  - Clean, intuitive UI built with NG-ZORRO components
  - Inline validation and error handling
  - Responsive design for seamless team collaboration
  - Real-time updates and instant feedback

---

## 🛠 Tech Stack

| Technology | Version | Purpose |
|------------|---------|---------|
| **Angular** | 17+ | Core framework |
| **TypeScript** | ~5.3 | Type-safe development |
| **NG-ZORRO** | ~17.4 | Enterprise UI components |
| **RxJS** | ~7.8 | Reactive programming |
| **HTML2Canvas** | ~1.4 | Screenshot/export functionality |
| **jsPDF** | ~3.0 | PDF generation |
| **Reactive Forms** | Built-in | Form management |
| **Standalone Components** | Built-in | Modern Angular architecture |

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** (v18 or higher recommended)
- **npm** (v9 or higher)
- **Angular CLI** (v17 or higher)

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd Weekly-report-management
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```

4. **Open in browser**
   Navigate to `http://localhost:4200/` in your web browser. The application will automatically reload when you modify any source files.

---

## 📝 Available Scripts

| Command | Description |
|---------|-------------|
| `npm start` | Start the development server at `http://localhost:4200/` |
| `npm run build` | Build the project for production in the `dist/` directory |
| `npm run watch` | Build in watch mode with hot-reload during development |
| `npm test` | Run unit tests via Karma |

---

## 💡 Usage

### Adding Team Members

1. Navigate to the **Team Settings** section
2. Click the "Add Member" button
3. Enter member details and assign a role
4. Confirm to add to your team

### Creating Tasks

1. Select a team member from the dashboard
2. Click "Add Task" for that member
3. Fill in the task details:
   - **Module Name**: Component or feature name
   - **Description**: Detailed task description
   - **Priority**: Select Low, Medium, or High
   - **Progress**: Drag the slider to indicate completion percentage
   - **Blocker**: Note any blockers or impediments
4. Save the task

### Tracking Progress

- View all team tasks in the **Task List** component
- Update progress sliders in real-time
- Weekly reports are automatically saved to your browser's LocalStorage
- Access historical data anytime without internet connectivity

---

## 📁 Project Structure

```
src/
├── app/
│   ├── components/
│   │   ├── add-member/          # Team member management
│   │   ├── add-task/            # Task creation and editing
│   │   ├── task-list/           # Task list and overview
│   │   ├── team-setting/        # Team configuration
│   │   └── weekly-report/       # Weekly report generation
│   ├── models/
│   │   ├── employee.model.ts    # Employee data structure
│   │   └── team.model.ts        # Team configuration model
│   ├── services/
│   │   ├── employee/            # Employee data management
│   │   ├── task/                # Task operations
│   │   └── team-setup/          # Team setup and configuration
│   ├── app.config.ts            # App configuration
│   ├── app.routes.ts            # Application routing
│   └── app.component.ts         # Root component
├── assets/                       # Static assets and images
├── styles.scss                  # Global styles
└── main.ts                      # Application entry point
```

---

## 🔧 Configuration

The application uses **Angular Standalone Components** architecture. Configuration is managed through:

- **`app.config.ts`**: Application-wide configuration and provider setup
- **`app.routes.ts`**: Route definitions for navigation
- **Environment variables**: Managed via Angular's environment files (if applicable)

### Data Storage

All data is persisted to the browser's **LocalStorage** under specific keys. Clearing browser data will reset the application state.

---

## 🎯 Key Features in Detail

### Weekly Report Generation

- Generate comprehensive weekly reports for individual team members
- Export reports as PDF for archival and sharing
- Track completion rates and blockers across the week

### Priority Management

Tasks are organized by priority levels to help teams focus on high-impact work:
- **High**: Critical path items requiring immediate attention
- **Medium**: Regular development tasks
- **Low**: Nice-to-have features or documentation

### Progress Tracking

- Real-time progress updates with percentage-based slider
- Visual indicators for task completion status
- Historical tracking of progress over time

---

## 🧪 Testing

Run the test suite to ensure code quality:

```bash
npm test
```

Tests are configured using:
- **Jasmine**: Testing framework
- **Karma**: Test runner
- **Chrome**: Default test browser

---

## 🏗️ Building for Production

Create a production build optimized for deployment:

```bash
npm run build
```

The build artifacts are stored in the `dist/` directory and can be deployed to any static hosting service (Vercel, Netlify, GitHub Pages, etc.).

---

## 📦 Dependencies

All dependencies are listed in `package.json`. Key libraries include:

- **@angular/\***: Core Angular framework and modules
- **ng-zorro-antd**: Enterprise-grade UI component library
- **rxjs**: Reactive programming library
- **html2canvas & jspdf**: Report export functionality

To install or update dependencies:

```bash
npm install
npm update
```

---

## 🚀 Deployment

The application is configured for easy deployment to **Vercel** using the included `vercel.json` configuration file.

### Deploy to Vercel

1. Install Vercel CLI: `npm i -g vercel`
2. Run: `vercel`
3. Follow the prompts to complete deployment

For other platforms, simply build the project and deploy the `dist/` directory to your hosting service.



## 🤝 Contributing

Contributions are welcome! Feel free to:

- Report issues and suggest features
- Submit pull requests with improvements
- Help improve documentation

---

## 📞 Support

For issues, questions, or feature requests, please open an issue in the repository or contact the development team.

---

**Built with ❤️ **