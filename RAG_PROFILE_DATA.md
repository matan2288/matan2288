# Matan's GitHub Profile - RAG Knowledge Base

**Generated:** 2026-06-03

---

## 👤 Profile Overview

- **Username:** matan2288
- **Profile Type:** Full-Stack Developer
- **GitHub:** https://github.com/matan2288
- **Social Links:** 
  - LinkedIn: https://linkedin.com/in/matan2288
  - Twitter: https://twitter.com/matan2288
  - Instagram: https://www.instagram.com/matan2288

---

## 🛠️ Core Technology Stack

### Frontend Technologies
- **Languages:** TypeScript, JavaScript
- **Frameworks & Libraries:** React, React Native, Vue.js, Svelte, Next.js patterns
- **State Management:** Redux, Redux Toolkit, Zustand patterns
- **Styling:** Tailwind CSS, Sass, CSS Modules
- **Component Libraries:** Storybook, Custom components with error handling
- **Build Tools:** Vite, Webpack, Expo Metro

### Backend Technologies
- **Languages:** TypeScript, JavaScript, Java
- **Frameworks:** 
  - Node.js + Express
  - Fastify (with TypeScript)
  - Firebase (authentication)
- **Databases:** MongoDB, MySQL
- **APIs:** GraphQL, REST, Convex (backend-as-a-service)
- **Deployment:** EAS Build (Expo), Vercel patterns

### Mobile Development
- **React Native** with Expo SDK 54
- **EAS Build** for iOS and Android builds
- **Expo Dev Client**
- **React Navigation** for mobile routing
- **Native Modules:** expo-location, react-native-maps, react-native-web

### DevTools & Infrastructure
- **Version Control:** Git
- **Package Managers:** npm
- **Code Quality:** ESLint, Prettier, TypeScript strict mode
- **Documentation:** Storybook, Mermaid diagrams
- **Build Automation:** npm scripts, Vite, tsc

### Languages Known
- TypeScript (Advanced)
- JavaScript (Advanced)
- Java (Intermediate-Advanced)
- Shell/Bash (Intermediate)
- Python (Basic - Data Analysis)
- C# (Intermediate)
- SQL (MySQL)

---

## 📚 Repository Catalog

### 1. Data Structures & Algorithms (Educational)

**Repository:** `data-structures-and-algorithms-2026`
- **Language:** Java
- **Type:** College Course Materials
- **Topics:**
  - Part 1: Records and Linked Lists
    * Java Records for immutable data classes
    * Node structure and linked list implementations
    * Traversal and insertion/deletion operations
    * Time complexity: O(1) head operations vs O(n) access
  - Part 2: Recursion
    * Base cases and recursive step patterns
    * Call stack mental models
    * Recursion on linked lists
    * When to prefer iteration vs recursion
  - Part 3: Binary Trees
    * Binary Tree fundamentals (root, leaf, height, depth)
    * Binary Search Trees (BST) with ordering invariant
    * Delete operations (0, 1, 2 children cases)
    * Tree traversals: Pre-order, In-order, Post-order
    * AVL Trees (self-balancing with rotation)
    * Balance factors and 4 rotation cases (LL, LR, RR, RL)
    * Almost Complete Binary Trees & Heaps
    * Array representation with index formulas
    * Min-heap property and bubble up/down operations
- **File Structure:**
  - Topics/Part 1 - Records and Linked Lists/README.md
  - Topics/Part 2 - Recursion/README.md
  - Topics/Part 3 - Binary Trees/README.md
    - 01_BinaryTree/BinaryTree.mmd (Mermaid diagrams)
    - 01_BinaryTree/01_BinaryTreeNodeExample.java
    - 02_Traversals/Traversals.mmd
    - 02_Traversals/02_BinaryTreeTraversalExample.java
    - 03_BST/BST.mmd
    - 03_BST/03_BSTExample.java
    - 04_AVL/AVL.mmd
    - 04_AVL/04_AVLExample.java
    - 05_Heap/Heap.mmd
    - 05_Heap/05_HeapExample.java

---

### 2. Rex SDK - React Component Library

**Repository:** `rex-sdk`
- **Language:** TypeScript
- **Type:** Reusable Component Library / Boilerplate
- **Purpose:** Production-ready component library with Storybook
- **Tech Stack:**
  - React 18.2.0+
  - TypeScript 5.2.2+
  - Vite 7.3.0 (bundler)
  - Storybook 9.1.1 (component documentation)
  - Tailwind CSS 3.4.3 (styling)
  - ESLint + Prettier (code quality)
- **Key Features:**
  - Type-safe component exports
  - Tailwind CSS integration with watch mode
  - Storybook for interactive component docs
  - CSS build separation (dist/styles.css)
  - Library publishing setup (UMD + ES modules)
- **Package Exports:**
  ```json
  {
    "import": "./dist/ui.es.js",
    "require": "./dist/ui.umd.js",
    "styles": "./dist/styles.css"
  }
  ```
- **Key Scripts:**
  - `npm run dev` - Development server
  - `npm run build` - Build library + CSS
  - `npm run build:css` - Tailwind CSS compilation
  - `npm run storybook` - Development storybook (port 6006)
  - `npm run build-storybook` - Static storybook export
  - `npm run format` - Code formatting
  - `npm run lint` - ESLint checking
- **Dependencies:**
  - @heroicons/react (icon library)
  - clsx (classname utility)
- **Dev Stack:**
  - Concurrently (parallel tasks)
  - Vite plugins (React, DTS)
  - Storybook addons (docs, links, onboarding, chromatic)

---

### 3. React Native Expo Boilerplate

**Repository:** `react-native-expo-boilerplate`
- **Language:** TypeScript
- **Type:** Mobile App Boilerplate
- **Purpose:** Minimal React Native starter with best practices
- **Versions:**
  - React Native 0.81.5
  - Expo 54.0.0
  - React 19.1.0
  - TypeScript 5.3.3
- **Key Features:**
  - Cross-platform support (iOS, Android, Web)
  - React Navigation integration
  - Safe area context handling
  - EAS Build configuration for production
- **Project Structure:**
  ```
  src/
  ├── app/          # Navigation & routing
  ├── features/     # Feature modules (auth, profile, orders, etc.)
  ├── shared/       # Reusable components, hooks, utilities
  ├── store/        # Global state (Redux/Zustand)
  ├── api/          # HTTP client setup with interceptors
  │   ├── client.ts - Axios/fetch instance
  │   └── endpoints.ts - API endpoint constants
  ├── theme/        # Design tokens (colors, spacing, typography)
  ├── assets/       # Images, fonts, icons
  └── types/        # Global TypeScript types
  
  Root config files:
  ├── app.json      # Expo configuration
  ├── babel.config.js
  ├── eas.json      # EAS Build settings
  ├── metro.config.js
  ├── tsconfig.json
  └── package.json
  ```
- **Required Asset Files:**
  - `assets/icon.png` (1024x1024) - App icon
  - `assets/splash.png` (1284x2778) - Splash screen
  - `assets/adaptive-icon.png` (1024x1024) - Android adaptive icon
  - `assets/favicon.png` (48x48) - Web favicon
- **Build Commands:**
  - `npm start` - Start dev server (i for iOS, a for Android, w for web)
  - `npm run build:android` - APK for Android devices
  - `npm run build:ios` - IPA for iOS (requires Apple Developer account)
  - `npm run build:simulator` - Emulator builds
  - `npm run build:all` - Production builds
- **First-time Setup:**
  ```bash
  npm install -g eas-cli
  eas login
  eas build:configure
  ```
- **Dependencies:**
  - @react-navigation/native
  - @react-navigation/native-stack
  - expo (all modules)
  - react-native-safe-area-context
  - react-native-screens
  - expo-dev-client
  - expo-status-bar

---

### 4. Rex Base - Advanced Boilerplate (In Progress)

**Repository:** `rex-base`
- **Language:** TypeScript
- **Type:** Advanced Full-Stack Boilerplate Template
- **Status:** Planning/Development Phase
- **Planned React Features:**
  - Error boundary implementation
  - Page wrapper with automatic routing
  - Redux Toolkit code generator
  - Automatic route/redux slice generation
  - Tailwind CSS styling
  - Header & footer components
  - Loading states
  - State persistence layer
  - Global keys and constants
  - Dark mode support
  - Separate Storybook instance
  - Translation infrastructure with AI generation
  - Build automation for Redux slice creation
- **Planned Express Backend:**
  - Firebase authentication (login)
  - Error handling middleware
  - API path constants
  - Environment variable conventions
  - Hot reload for custom JavaScript
- **Deployment Considerations:** Yes (to be added)
- **Base Tech:** React + TypeScript + Vite

---

### 5. Fastify Node.js TypeScript Base Template

**Repository:** `fastify-nodejs-ts-base-template`
- **Language:** TypeScript
- **Type:** Backend API Boilerplate
- **Purpose:** Minimal Node.js API starter with Fastify
- **Versions:**
  - Fastify 4.24.3
  - TypeScript 5.2.2
  - Node.js compatible
- **Key Dependencies:**
  - fastify (HTTP framework)
  - typescript (type safety)
  - ts-node (TypeScript execution)
  - nodemon (watch mode)
- **Key Scripts:**
  - `npm start` - Compile & run with watch mode (nodemon + ts-node)
  - `npm run build` - TypeScript compilation to JavaScript
- **Project Structure:**
  - `src/index.ts` - Entry point
- **Use Case:** Quick API backend setup

---

### 6. Dirot - Yad2 Property Listings App

**Repository:** `Dirot`
- **Language:** TypeScript
- **Type:** Production Mobile Application
- **Purpose:** Real estate property listings aggregator from Yad2 API
- **Tech Stack:**
  - React Native 0.81.5
  - Expo 54.0.0
  - Convex (backend-as-a-service)
  - React 19.1.0
  - TypeScript 5.3.3
- **Features:**
  - Fetch properties from Yad2 API
  - Convex cloud database
  - Property filtering (price, rooms, area)
  - Pull-to-refresh functionality
  - Property cards with images and details
  - Responsive mobile UI
- **Project Structure:**
  ```
  ├── App.tsx                 # Main app with Convex provider
  ├── components/
  │   ├── PropertyList.tsx    # List display
  │   ├── PropertyCard.tsx    # Card component
  │   └── FetchButton.tsx     # API fetch trigger
  ├── convex/
  │   ├── schema.ts           # Database schema
  │   ├── fetchProperties.ts  # Queries & mutations
  │   └── _generated/         # Auto-generated files
  ├── convexUrl.ts            # Deployment URL config
  ├── app.json                # Expo config
  ├── eas.json               # EAS Build config
  └── metro.config.js
  ```
- **Convex Setup:**
  ```bash
  npm install -g convex
  npx convex login
  npx convex dev
  ```
- **Default API Filters:**
  - City: 5000 (Tel Aviv)
  - Neighborhood: 485
  - Area: 1, Top Area: 2
  - Price range: 5000-10000
  - Rooms: 2-4
- **Additional Dependencies:**
  - convex (backend)
  - expo-location (location services)
  - react-native-maps (mapping)
  - react-native-url-polyfill (polyfill)

---

### 7. Full-Stack Table App (React + Express)

**Repository:** `fs_table_app_react_express1532`
- **Language:** JavaScript / React
- **Type:** Full-stack CRUD Application
- **Purpose:** Table data management with React frontend + Express backend
- **Architecture:**
  - `ui/` - React + Vite frontend
  - `server/` - Express backend
- **Frontend Setup:**
  - React with Vite
  - ESLint configuration
- **Use Case:** Data table display and manipulation

---

### 8. Flappy Bird Game (Java Swing)

**Repository:** `flappy_bird_java_swing1532`
- **Language:** Java
- **Type:** Game Implementation
- **Framework:** Java Swing
- **Purpose:** Classic Flappy Bird game clone

---

### 9. Flappy Bird Game (React Native TypeScript)

**Repository:** `flappy_bird_rntv_1532`
- **Language:** TypeScript
- **Type:** Game Implementation
- **Framework:** React Native
- **Purpose:** Cross-platform Flappy Bird

---

### 10. Flappy Bird Game (Java)

**Repository:** `flappy_bird524_java`
- **Language:** Java
- **Type:** Game Implementation
- **Framework:** Java Swing
- **Purpose:** Another Flappy Bird implementation variant

---

### 11. Advanced Java College Training

**Repository:** `adavanced_java_clg_2025`
- **Language:** Java
- **Type:** Educational Material
- **Purpose:** Advanced Java concepts for college course

---

### 12. Shell & Regex Training

**Repository:** `shell_regex_training_clg2026`
- **Language:** Shell (Bash)
- **Type:** Educational Material
- **Purpose:** Unix shell scripting and regular expressions

---

### 13. React Native Expo Boilerplate (Additional)

**Repository:** `react-native-expo-boilerplate`
- **Language:** TypeScript
- **Description:** See detailed section above

---

### 14. C# College Training

**Repository:** `cshap_college_training`
- **Language:** C#
- **Type:** Educational Material
- **Purpose:** C# programming language training

---

### 15. Front-End Interview Training

**Repository:** `fe_interview_training`
- **Language:** JavaScript
- **Type:** Educational / Practice
- **Purpose:** Preparation for front-end developer interviews

---

### 16. Desktop App Boilerplate (Java Swing)

**Repository:** `desktop-app-boilerplate-java-swing231`
- **Language:** Java
- **Type:** Boilerplate
- **Framework:** Java Swing
- **Purpose:** Desktop GUI application starter template

---

### 17. Desktop App Boilerplate (Another)

**Repository:** `cursor_settings_matan`
- **Type:** Configuration / Settings
- **Purpose:** Cursor IDE configuration and preferences

---

### 18. Apex Test

**Repository:** `Apex-test`
- **Language:** TypeScript
- **Type:** Test/Experiment
- **Description:** "test"
- **Purpose:** Salesforce Apex testing or general TypeScript testing

---

### 19. N8N Automation

**Repository:** `N8N`
- **Language:** JavaScript
- **Type:** Automation Setup
- **Purpose:** N8N workflow automation platform setup

---

### 20. Dirot (Already Listed)

**Repository:** `Dirot`
- See detailed section above

---

### 21. Data Analysis Mid-Semester Project

**Repository:** `data-analysis-mid-semester-project`
- **Language:** Jupyter Notebook / Python
- **Type:** Academic Project
- **Purpose:** Data analysis coursework

---

### 22. UI Scripts Base

**Repository:** `ui_scripts_base`
- **Language:** JavaScript/TypeScript (unspecified)
- **Type:** Utility Library
- **Description:** General UI scripts for UI applications
- **Purpose:** Reusable UI automation scripts

---

### 23. MySQL Playground

**Repository:** `mysql_playground_5123`
- **Language:** Mermaid (SQL Diagrams)
- **Type:** Learning/Practice
- **Purpose:** MySQL database design and practice

---

### 24. Rex Base (Already Listed)

**Repository:** `rex-base`
- See detailed section above

---

### 25. C# College Training (Already Listed)

**Repository:** `cshap_college_training`
- See above

---

### 26. Matan's Portfolio

**Repository:** `matan2288_portfolio`
- **Language:** CSS
- **Type:** Personal Website
- **Purpose:** Showcase of skills and projects

---

### 27. Full-Stack Table App (Already Listed)

**Repository:** `fs_table_app_react_express1532`
- See above

---

### 28. Svelte Training

**Repository:** `svelte-training-aug24`
- **Language:** Svelte
- **Type:** Educational
- **Purpose:** Svelte framework learning

---

### 29. React TypeScript Custom Input Component

**Repository:** `react-ts-custom-input-component`
- **Language:** TypeScript
- **Type:** Component Library / Reusable Component
- **Description:** Custom input component with error handling
- **Purpose:** Reusable form input for projects
- **Features:** TypeScript typing, error states, validation support

---

### 30. Fastify Node.js TypeScript Base Template (Already Listed)

**Repository:** `fastify-nodejs-ts-base-template`
- See detailed section above

---

### 31. Fastify Training

**Repository:** `fastify-training`
- **Language:** JavaScript
- **Type:** Educational
- **Purpose:** Fastify framework learning and examples

---

### 32. GraphQL Training

**Repository:** `graphql-training`
- **Language:** JavaScript
- **Type:** Educational
- **Purpose:** GraphQL API development learning

---

### 33. JavaScript OOP Training

**Repository:** `javascript-oop-training`
- **Language:** JavaScript
- **Type:** Educational
- **Purpose:** Object-Oriented Programming in JavaScript

---

### 34. Utils Matan

**Repository:** `utils-matan`
- **Language:** JavaScript
- **Type:** Utility Library
- **Description:** General utils and rules
- **Purpose:** Reusable utility functions for projects
- **Export Style:** npm package

---

### 35. Etherscan Transaction Tracker

**Repository:** `EtherscanAccount-TransactionTracker-electron-reactapp`
- **Language:** Jupyter Notebook / TypeScript/JavaScript
- **Type:** Desktop Application
- **Purpose:** Blockchain account transaction tracking
- **Tech:** Electron + React
- **Use Case:** Monitor Ethereum transactions

---

### 36. Profile README

**Repository:** `matan2288` (Main profile repo)
- **Language:** Markdown
- **Type:** Profile Showcase
- **Content:**
  - GitHub stats and language distribution
  - Tech stack badges and icons
  - Social links
  - Professional presentation
- **Technologies Displayed:**
  - TypeScript, React, Redux
  - GraphQL, Vue.js, Sass
  - Tailwind CSS, Node.js, Express
  - MongoDB, MySQL, Git

---

## 🏗️ Architecture Patterns & Best Practices

### Frontend Patterns
1. **Feature-based folder structure** (src/features/*)
2. **Shared components** library (src/shared/*)
3. **Centralized state management** (Redux, Zustand)
4. **API layer abstraction** (client.ts, endpoints.ts)
5. **Theme/Design system** (colors, spacing, typography)
6. **Type safety** - TypeScript for all React projects
7. **Storybook documentation** - Component-driven development
8. **Error boundaries** - Error handling in React
9. **Safe area handling** - Mobile-specific (React Native)

### Backend Patterns
1. **TypeScript for type safety**
2. **Environment-based configuration**
3. **Error handling middleware**
4. **API endpoint constants**
5. **Firebase authentication integration**
6. **Database abstraction layers**

### Code Quality
- **ESLint** - Code linting
- **Prettier** - Code formatting
- **TypeScript strict mode** - Type safety
- **Pre-commit hooks** - Code quality gates

### Build & Deployment
- **Vite** for frontend bundling
- **npm scripts** for automation
- **EAS Build** for mobile CI/CD
- **Storybook** for component documentation

---

## 📊 Technology Statistics

### By Language
| Language | Count | Primary Use |
|----------|-------|-------------|
| TypeScript | 12+ | React, React Native, Node.js, Fastify |
| JavaScript | 8+ | React, Node.js, Training |
| Java | 5 | DSA, Games, Desktop apps |
| Shell | 1 | Scripting, Training |
| Python | 1 | Data Analysis |
| C# | 1 | Training |
| Svelte | 1 | Training |
| CSS | 1 | Portfolio |
| Mermaid | 1 | Diagrams |
| Jupyter | 2 | Data analysis, Blockchain |

### By Project Type
| Type | Count | Examples |
|------|-------|----------|
| Boilerplate/Template | 5 | rex-sdk, react-native-expo-boilerplate, fastify-template |
| Educational | 8 | DSA, JavaScript OOP, GraphQL, Svelte |
| Production Apps | 3 | Dirot, Transaction Tracker, Portfolio |
| Games | 3 | Flappy Bird (3 variants) |
| Utility Libraries | 3 | utils-matan, ui_scripts_base, custom-input |
| Full-Stack Projects | 2 | Table app, Dirot |
| Configuration | 1 | Cursor settings |

### Most Used Dependencies
- React & React Native
- TypeScript
- Vite
- Tailwind CSS
- Expo & EAS
- Express
- Fastify
- Redux (patterns)
- Storybook
- ESLint & Prettier

---

## 🎯 Preferred Developer Workflow

### Development
1. TypeScript first (for type safety)
2. Component-driven with Storybook
3. Feature-based architecture
4. Centralized state management
5. API layer abstraction

### Code Quality
1. ESLint for linting
2. Prettier for formatting
3. TypeScript strict mode
4. Error handling boundaries

### Build Tools
1. Vite for bundling
2. npm scripts for automation
3. Environment-based configuration

### Deployment
1. Mobile: EAS Build (iOS/Android)
2. Web: Vercel patterns (Vite)
3. Backend: Node.js (Express/Fastify)

---

## 💾 Common Project Conventions

### Folder Structure (Frontend)
```
src/
├── app/                    # App entry & navigation
├── features/              # Feature modules
├── shared/               # Shared components & hooks
├── store/                # State management
├── api/                  # API client & endpoints
├── theme/                # Design system
├── assets/               # Static files
├── types/                # TypeScript types
└── constants/            # Global constants
```

### Naming Conventions
- Component files: PascalCase (e.g., `PropertyCard.tsx`)
- Utility files: camelCase (e.g., `client.ts`)
- Constants: UPPER_SNAKE_CASE
- Folders: kebab-case or camelCase (feature-based)

### Package Script Patterns
```json
{
  "start": "development server",
  "build": "production build",
  "dev": "development with watch",
  "lint": "code linting",
  "format": "code formatting",
  "storybook": "component documentation",
  "test": "unit tests (when applicable)"
}
```

---

## 🔑 Key Skills & Expertise Areas

### Strong Areas
- React & React Native development
- TypeScript type systems
- Mobile development (Expo, EAS)
- Component design and Storybook
- Full-stack JavaScript/TypeScript
- API design (REST, GraphQL)
- UI/UX implementation (Tailwind CSS, Sass)

### Intermediate Areas
- Java (data structures, design patterns)
- Database design (MongoDB, MySQL)
- DevOps fundamentals (EAS, Git)
- State management (Redux patterns)

### Learning Areas
- C#
- Svelte
- Advanced data analysis
- Blockchain/Web3

---

## 📞 How to Use This Document for RAG

This document serves as your personal knowledge base. Use it to:

1. **Query development patterns**: "What folder structure does Matan use?"
2. **Technology recommendations**: "What tools does Matan prefer for mobile development?"
3. **Project templates**: "Which boilerplate should I use for X?"
4. **Learning resources**: "What educational repos exist for topic Y?"
5. **Code standards**: "What are Matan's coding conventions?"
6. **Dependency choices**: "Which libraries does Matan commonly use?"

---

**Last Updated:** 2026-06-03
**Total Repositories:** 30+
**Active Projects:** Multiple (learning + production)
**Profile Status:** Active Developer
