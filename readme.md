整体效果：



https://github.com/user-attachments/assets/0f8e33b0-984d-4e7d-8257-9a2cd971a033


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

   a. 访问 api.useaihub.com 注册账号并获取 API 密钥。

   b. 在已部署的 Lobe Chat 中,打开设置。

   c. 在 "OpenAI API 设置" 部分:
      - API 密钥: 输入从 api.useaihub.com 获取的 API 密钥
      - API 接口地址: 输入 https://api.useaihub.com/v1

   d. 保存设置。
   
   e. 加我wc通知我改群组，开放更多模型!
   
   <img src="https://github.com/user-attachments/assets/c23dc989-c605-44f2-8df7-b17dfc84a079" width="80" height="80">


4. 开始使用:
   现在你可以开始使用 Lobe Chat,它将通过你在 api.useaihub.com 的账户访问 OpenAI 的服务。

