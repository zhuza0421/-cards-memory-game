# Cards Memory Game Installation and Deployment Guide
# 卡牌记忆游戏安装与部署指南

## Prerequisites
## 环境要求
Before you begin, ensure you have the following installed:
在开始前，请确保已安装以下软件：
- Git
- Node.js and npm (Node package manager)
- Node.js 和 npm (Node包管理器)

## Installation Steps
## 安装步骤
### 1. Clone the Repository
### 1. 克隆代码仓库
Open a terminal and run the following command to clone the repository:
打开终端并运行以下命令克隆仓库：
```bash
git clone https://github.com/dsydai/-cards-memory-game.git
```

### 2. Install Dependencies
### 2. 安装依赖项
Navigate to the project directory and run the following command to install the required dependencies:
#进入项目目录并运行以下命令安装所需依赖：
```bash
cd -cards-memory-game
npm install
```

## Project Structure
## 项目结构
The project structure is as follows:
项目结构如下：
```
-cards-memory-game/
├── public/               # 公共文件夹
│   ├── index.html        # HTML模板
│   └── ...               # 其他公共文件
├── src/                  # 源代码文件夹
│   ├── components/       # 所有React组件
│   ├── App.js            # 主应用组件
│   ├── App.test.js       # App组件测试文件
│   ├── index.css         # 全局CSS文件
│   ├── index.js          # React应用入口文件
│   └── ...               # 其他源文件
├── .gitignore            # 指定Git忽略的文件
├── package.json          # 管理项目依赖和脚本
├── package-lock.json     # 锁定依赖版本以确保一致性
├── README.md             # 项目文档文件
└── ...                   # 其他文件和目录
```

## Deployment Steps
## 部署步骤
### Running in Development Mode
### 开发模式运行
1. Install live-server:
#1. 安装live-server:
```bash
npm install -g live-server
```
2. Start the development server:
2. 启动开发服务器:
```bash
live-server
```
3. The browser will automatically open `http://localhost:8080`
3. 浏览器将自动打开 `http://localhost:8080`

### Server Deployment
### 服务器部署
1. Upload the project files to the web server's root directory (e.g., Apache/Nginx)
#1. 将项目文件上传到Web服务器的根目录（如Apache/Nginx）
2. Ensure the `index.html` file is accessible via the URL
#2. 确保可以通过URL访问`index.html`文件
