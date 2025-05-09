# Cards Memory Game Installation and Deployment Guide

## Prerequisites
Before you begin, ensure you have the following installed:
- Git
- Node.js and npm (Node package manager)
## Installation Steps
### 1. Clone the Repository
Open a terminal and run the following command to clone the repository:
```bash
git clone https://github.com/dsydai/-cards-memory-game.git
```
### 2. Install Dependencies
Navigate to the project directory and run the following command to install the required dependencies:
```bash
cd -cards-memory-game
npm install
```
## Project Structure
The project structure is as follows:
```
-cards-memory-game/
├── public/
│   ├── index.html  # HTML template
│   └── ...         # Other public files
├── src/
│   ├── components/ # All React components
│   ├── App.js      # Main application component
│   ├── App.test.js # Test file for App component
│   ├── index.css   # Global CSS file
│   ├── index.js    # Entry point for the React application
│   └── ...         # Other source files
├── .gitignore      # Specifies untracked files to be ignored by Git
├── package.json    # Manages project dependencies and scripts
├── package-lock.json # Locks dependency versions for consistent installation
├── README.md       # Project documentation file
└── ...             # Other files and directories
```
## Deployment Steps
### Running in Development Mode
1. Install live-server:
```bash
npm install -g live-server
```
2. Start the development server:
```bash
live-server
```
3. The browser will automatically open `http://localhost:8080`

### Server Deployment
1. Upload the project files to the web server's root directory (e.g., Apache/Nginx)
2. Ensure the `index.html` file is accessible via the URL

<!-- by dengsiyu  -->