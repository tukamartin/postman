# Postman tasks

### Install Postman CLI with these commands

Windows

powershell.exe -NoProfile -InputFormat None -ExecutionPolicy AllSigned -Command "[System.Net.ServicePointManager]::SecurityProtocol = 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://dl-cli.pstmn.io/install/win64.ps1'))"

Linux

curl -o- "https://dl-cli.pstmn.io/install/linux64.sh" | sh

Mac (Apple silicon) installation

curl -o- "https://dl-cli.pstmn.io/install/osx_arm64.sh" | sh

### Clone tasks to folder you selected

git clone https://github.com/tukamartin/postman.git

### Run task 1

postman collection run "postman/Postman Collections/api_task_1.json"

### Run task 2

postman collection run "postman/Postman Collections/api_task_2.json" -d "postman/Postman Collections/users.csv"
