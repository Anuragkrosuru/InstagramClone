# Instagram Clone
Instagram Clone Demo

A full-featured Instagram clone built with client-side dynamic pages using React and Flask, demonstrating modern web development techniques including AJAX, REST APIs, and asynchronous programming.

<img width="481" height="540" alt="image" src="https://github.com/user-attachments/assets/6abbbc4f-8b1f-40dd-a6ed-4f4963dd0e14" />

## 🎯 Learning Goals

- **Client-side Dynamic Pages**: React-based user interface with JavaScript
- **Asynchronous Programming**: AJAX calls and state management
- **REST API Development**: Backend API for data operations
- **Modern Web Technologies**: React Hooks, Webpack, and modern JavaScript

## 🏗️ Architecture Overview

This project transforms a server-side Instagram clone into a client-side application with three main components:

1. **Flask Backend** - REST API endpoints and server-side authentication
2. **React Frontend** - Client-side dynamic pages with state management
3. **Database Layer** - SQLite database for user data, posts, likes, and comments

## 🛠️ Tech Stack

### Backend
- **Python**: Flask web framework
- **Database**: SQLite with custom schema
- **Authentication**: Session-based and HTTP Basic Auth
- **API**: RESTful endpoints for posts, likes, and comments

### Frontend
- **React**: Modern JavaScript framework with Hooks
- **Webpack**: JavaScript bundler and build tool
- **CSS**: Styling with modern CSS features
- **State Management**: React useState and useEffect hooks

### Development Tools
- **ESLint**: JavaScript code linting
- **Prettier**: Code formatting
- **Cypress**: End-to-end testing
- **TypeScript**: Optional type-safe JavaScript

## 📁 Project Structure

```
p3-insta485-clientside/
├── bin/                    # Shell scripts (install, run, test, database)
├── insta485/              # Main Flask application
│   ├── __init__.py        # Flask app initialization
│   ├── config.py          # Configuration settings
│   ├── model.py           # Database models and queries
│   ├── api/               # REST API endpoints
│   │   ├── __init__.py
│   │   ├── posts.py       # Post-related API routes
│   │   ├── likes.py       # Like-related API routes
│   │   └── comments.py    # Comment-related API routes
│   ├── views/             # Server-side page routes
│   ├── templates/         # HTML templates
│   ├── static/            # Static files (CSS, images)
│   └── js/                # React components
│       ├── main.jsx       # Main React entry point
│       └── post.jsx       # Post component
├── sql/                   # Database schema and data
│   ├── schema.sql         # Database structure
│   ├── data.sql           # Sample data
│   └── uploads/           # Image uploads
├── tests/                 # Test suite
│   └── cypress/           # End-to-end tests
├── package.json           # JavaScript dependencies
├── webpack.config.js      # Webpack configuration
└── requirements.txt       # Python dependencies
```

## 🔍 Core Features

### Instagram-like Functionality
- **User Authentication**: Login/logout with session management
- **Post Feed**: Infinite scroll with dynamic loading
- **Like System**: Real-time like/unlike without page reload
- **Comment System**: Add/delete comments with instant updates
- **User Profiles**: View user posts and follow relationships
- **Image Uploads**: Handle profile pictures and post images

### Client-side Dynamic Features
- **Real-time Updates**: Likes and comments update instantly
- **Infinite Scroll**: Load more posts as user scrolls
- **Double-click to Like**: Instagram-style image interaction
- **Responsive Design**: Mobile-friendly interface
- **State Management**: React-based component state

### REST API Endpoints
- **GET /api/v1/** - API resource discovery
- **GET /api/v1/posts/** - Retrieve post feed with pagination
- **GET /api/v1/posts/<id>/** - Get specific post details
- **POST /api/v1/likes/** - Create new like
- **DELETE /api/v1/likes/<id>/** - Remove like
- **POST /api/v1/comments/** - Add comment
- **DELETE /api/v1/comments/<id>/** - Remove comment

## 🚀 Getting Started

### Prerequisites
```bash
python 3.8+
node.js 14+
npm or yarn
sqlite3
```

### Installation
```bash
# Clone the repository
git clone [your-repo-url]
cd p3-insta485-clientside

# Run install script
./bin/insta485install

# Activate virtual environment
source env/bin/activate

# Generate database
./bin/insta485db reset
```

### Running the Application
```bash
# Start development server (builds frontend and starts Flask)
./bin/insta485run

# Access the application
# http://localhost:8000
```

## 📊 Key Features

### Authentication System
- **Session Management**: Flask session-based authentication
- **HTTP Basic Auth**: REST API authentication support
- **User Registration**: Account creation and management
- **Secure Routes**: Protected endpoints for authenticated users

### Post Management
- **Feed Generation**: Algorithm-based post ordering
- **Pagination**: Efficient loading of large post collections
- **Image Handling**: Upload and display of post images
- **Timestamp Display**: Human-readable relative time formatting

### Interactive Features
- **Like Functionality**: Toggle likes with immediate UI updates
- **Comment System**: Real-time comment addition and deletion
- **Double-click Interaction**: Instagram-style image liking
- **Infinite Scroll**: Seamless post loading experience

## 🧪 Testing

### Backend Testing
```bash
# Run Python unit tests
pytest -v

# Style checks
pycodestyle -v insta485
pydocstyle -v insta485
pylint -v insta485
```

### Frontend Testing
```bash
# JavaScript style checks
npx eslint --ext jsx insta485/js/
npx prettier --check insta485/js

# End-to-end testing
npx cypress open
npx cypress run
```

### Full Test Suite
```bash
# Run all tests including style checks
./bin/insta485test
```

## 📈 Performance Features

- **Client-side Rendering**: Fast UI updates without server round-trips
- **Efficient API Calls**: Minimal data transfer with REST endpoints
- **Image Optimization**: Optimized image handling and display
- **State Management**: Efficient React state updates and re-renders

## 🔧 Development Features

- **Hot Reloading**: Webpack watch mode for automatic rebuilds
- **Modern JavaScript**: ES6+ features and React Hooks
- **Code Quality**: ESLint and Prettier for consistent code style
- **Type Safety**: Optional TypeScript support for better development experience

## 🚀 Deployment

### AWS Deployment
- **EC2 Instance**: Cloud-based hosting
- **Nginx Configuration**: Production web server setup
- **Gunicorn**: WSGI server for Flask application
- **Static File Serving**: Optimized delivery of JavaScript bundles

### Production Build
```bash
# Build production JavaScript bundle
npx webpack --mode production

# Deploy to AWS using provided scripts
# Follow AWS deployment tutorial
```

## 📝 Project Requirements

- **Group Project**: Teams of 2-3 students
- **Due Date**: 11:59pm ET February 16, 2025
- **Submission**: Tarball with source code and deployment artifacts
- **Testing**: Must pass all public and hidden unit tests

## 🎨 Code Style

### Python Code
- **PEP 8 Compliance**: pycodestyle validation
- **Documentation**: pydocstyle compliance
- **Code Quality**: pylint analysis

### JavaScript Code
- **AirBnB Style**: ESLint with AirBnB configuration
- **Formatting**: Prettier automatic formatting
- **React Best Practices**: Modern React patterns and hooks

## 👨‍💻 Author

**Anurag Krosuru**
- GitHub: [@Anuragkrosuru](https://github.com/Anuragkrosuru)
- LinkedIn: [anuragkro](https://www.linkedin.com/in/anuragkro)
- Course: EECS 485 - Web Systems, University of Michigan

## 🙏 Acknowledgments

- **Course Staff**: Andrew DeOrio, Noah Weingarden, EECS 485 Team
- **University of Michigan**: EECS 485 Course Materials
- **React Community**: Modern React development patterns
- **Web Development Tools**: Webpack, ESLint, Prettier, Cypress

---

⭐ **This project demonstrates modern web development techniques including client-side dynamic pages, REST APIs, and asynchronous programming with React and Flask.**



