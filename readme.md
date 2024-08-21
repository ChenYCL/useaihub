
# 如果您是其它行业的，这里有5分钟快速安装docker步骤：

## macOS 用户安装 Docker

1. 访问 [Docker 官网](https://www.docker.com/products/docker-desktop/)
2. 点击 "Download for Mac" 按钮
3. 下载完成后,双击 "Docker.dmg" 文件
4. 在打开的窗口中,将 Docker 图标拖拽到 Applications 文件夹
5. 打开 Applications 文件夹,双击 Docker 图标启动它
6. 首次启动时,系统可能会要求输入管理员密码,请输入并确认
7. Docker 启动后,顶部菜单栏会出现一个小鲸鱼图标
8. 打开 Terminal(终端),输入 `docker --version` 确认安装成功

## Windows 用户安装 Docker

1. 访问 [Docker 官网](https://www.docker.com/products/docker-desktop/)
2. 点击 "Download for Windows" 按钮
3. 下载完成后,双击运行 "Docker Desktop Installer.exe"
4. 在安装向导中,保持默认选项,点击 "Ok" 继续
5. 安装完成后,点击 "Close and restart" 重启电脑
6. 重启后,Docker 会自动启动。任务栏中会出现 Docker 图标
7. 首次运行可能会弹出提示,要求安装 WSL 2。按照提示完成安装
8. 打开 PowerShell 或命令提示符,输入 `docker --version` 确认安装成功

## 整体效果：

https://github.com/user-attachments/assets/0f8e33b0-984d-4e7d-8257-9a2cd971a033

## 如何使用

1. 部署 Lobe Chat:

   a. 访问 Lobe Chat 的 GitHub 仓库: https://github.com/lobehub/lobe-chat
   
   b. 选择一种部署方式:
      - 使用 Vercel 一键部署
      - 使用 Docker 部署

   c. 对于 Vercel 一键部署:
   
| Deploy with Vercel |
| :-----------------: |
| [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Flobehub%2Flobe-chat&project-name=lobe-chat&repository-name=lobe-chat) |

   d. 对于 Docker 部署:
      - 运行以下命令:
```bash
       docker run -d -p 3210:3210 \
        -e OPENAI_API_KEY=sk-xxxx \
        -e OPENAI_PROXY_URL=https://api.useaihub.com/v1 \
        -e ACCESS_CODE=lobe66 \
        --name lobe-chat \
        lobehub/lobe-chat
```

  - 访问 http://localhost:3210 使用 Lobe Chat


2. 配置 OpenAI 接口服务:

   a. 访问 api.useaihub.com 注册账号并获取 API 密钥（https://api.useaihub.com/token）。
<img width="1559" alt="image" src="https://github.com/user-attachments/assets/8fc882c4-1db2-463a-9ffc-fdec321caf13">


   b. 在已部署的 Lobe Chat 中,打开设置。

   c. 在 "OpenAI API 设置" 部分:
      - API 密钥: 输入从 api.useaihub.com 获取的 API 密钥
      - API 接口地址: 输入 https://api.useaihub.com/v1

   d. 保存设置。
   

4. 开始使用:
   现在你可以开始使用 Lobe Chat,它将通过你在 api.useaihub.com 的账户访问 OpenAI 的服务。

 ## 加入群组，联系我修改用户类别更多模型!
 https://github.com/user-attachments/assets/4bafc182-f842-46d0-b0cb-18eb113589b8
   
<img src="https://github.com/user-attachments/assets/4bafc182-f842-46d0-b0cb-18eb113589b8" width="200" height="300">


