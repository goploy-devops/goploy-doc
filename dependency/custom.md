# custom命令
使用系统支持的命令
```
  cmd := exec.Command("传输选项")
```

## 预定义变量

```
${PROJECT_ID}=           strconv.FormatInt(project.ID, 10)
${PROJECT_PATH}=         project.Path
${PROJECT_SYMLINK_PATH}= path.Join(project.SymlinkPath, project.LastPublishToken)
${PROJECT_NAME}=         project.Name
${PROJECT_BRANCH}=       project.Branch
${REPOSITORY_TYPE}=      project.RepoType
${REPOSITORY_URL}=       project.URL
${REPOSITORY_PATH}=      core.GetProjectPath(project.ID)
${PUBLISH_TOKEN}=        project.LastPublishToken
${SERVER_ID}=            strconv.FormatInt(server.ServerID, 10)
${SERVER_NAME}=          server.ServerName
${SERVER_IP}=            server.ServerIP
${SERVER_PORT}=          strconv.Itoa(server.ServerPort)
${SERVER_OWNER}=         server.ServerOwner
${SERVER_PASSWORD}=      server.ServerPassword
${SERVER_PATH}=          server.ServerPath
${SERVER_JUMP_IP}=       server.ServerJumpIP
${SERVER_JUMP_PORT}=     strconv.Itoa(server.ServerJumpPort)
${SERVER_JUMP_OWNER}=    server.ServerJumpOwner
${SERVER_JUMP_PASSWORD}= server.ServerJumpPassword
${SERVER_JUMP_PATH}=     server.ServerJumpPath
```
