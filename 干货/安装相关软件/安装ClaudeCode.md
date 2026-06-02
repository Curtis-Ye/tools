# ClaudeCode安装步骤(Linux)
## 1.首先更新系统环境:  
`sudo apt update && sudo apt upgrade -y `  
## 2.安装Node.js:  
`curl -fsSL https://deb.nodesource.com/setup_22.x | sudo -E bash -`  
`sudo apt install -y nodejs`  
## 3.安装Git(有安装过Git的不需要这一步)：  
`sudo apt install -y git`  
`git --version`  
## 4.安装 Claude Code CLI  
`npm install -g @anthropic-ai/claude-code`  
## 5.检查是否安装成功：  
`claude --version`  