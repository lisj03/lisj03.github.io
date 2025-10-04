---
title: copilot agent 的vscode 配置
---

### 设置maxrequests

- 设置里搜索copilot

  ![](<image/copilot agent 的vscode 配置/截屏2025-09-15 10.26.09_MyfAWQnNkg.png>)
- 打开settings.json

  添加3行内容
  ```json 
      "chat.agent.maxRequests":100,
      "chat.todoListTool.enabled": true,
      "chat.tools.autoApprove": true,
  ```

  ![](<image/copilot agent 的vscode 配置/截屏2025-09-15 10.27.51_jH5nHYgLSN.png>)

### 允许命令行运行命令

- comm +  ，
- 编辑settings.json文件
  ```json 
  "chat.tools.terminal.autoApprove": {


          "mkdir": true,
          "npm run build": true,
          "^git (status|show\\b.*)$": true,
          "^/Get-ChildItem\\b.*": true,
          "ls": true,
          "pwd": true,
          "cd": true,
          "rmdir": true,
          "chmod": true,
          "kill": true,
          "head":true,
          "bash": true,
          "tail":true,
          "conda":true,
          "python":true,
          "pip":true,
          "grep":true,
          "./*":true,

          "rm": false,
          "del": false,
          "curl": false,
          "wget": false,
          "eval": false,
          "chown": false,
          "/^Remove-Item\\b/i": false
      },
  ```


### Debug Log

![](<image/copilot agent 的vscode 配置/截屏2025-09-17 14.15.22_YKNQInNqm9.png>)
