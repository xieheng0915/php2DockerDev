使用Remote-Container extension打造vscode+remote container开发环境

这个插件可以实现vscode在container中打开，从而将vscode 和 container 无缝连接  

原理参看官方文档：https://code.visualstudio.com/docs/remote/containers  

- 安装remote-container 插件
- 建立Dockerfile, docker-compose.yml 
- 在terminal 中使用以下命令
```
docker build - < Dockerfile //可省略而直接用以下的docker-compose命令
docker-compose up --build  //要加上--build避免缺少的镜像
```
- 在vscode 中使用Remote-Containers：reopen in the container重新打开