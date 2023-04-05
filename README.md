<div align="center">
<img src="./static/icon.svg" alt="预览"/>

<h1 align="center">ChatGPT Next Web</h1>

一键免费部署你的私人 ChatGPT 网页应用。



[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Frandy7366%2FChatGPT-Next-Web&env=OPENAI_API_KEY&env=CODE&project-name=chatgpt-next-web&repository-name=ChatGPT-Next-Web)


![主界面](./static/cover.png)

</div>

## 主要功能

- 在 1 分钟内使用 Vercel **免费一键部署**
- 精心设计的 UI，响应式设计，支持深色模式
- 极快的首屏加载速度（~100kb）
- 海量的内置 prompt 列表，来自[中文](https://github.com/PlexPt/awesome-chatgpt-prompts-zh)和[英文](https://github.com/f/awesome-chatgpt-prompts)
- 自动压缩上下文聊天记录，在节省 Token 的同时支持超长对话
- 一键导出聊天记录，完整的 Markdown 支持
- 拥有自己的域名？好上加好，绑定后即可在任何地方**无障碍**快速访问

## 开始使用

1. 准备好你的 [OpenAI API Key](https://platform.openai.com/account/api-keys);
2. 点击右侧按钮开始部署：
   [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Frandy7366%2FChatGPT-Next-Web&env=OPENAI_API_KEY&env=CODE&project-name=chatgpt-next-web&repository-name=ChatGPT-Next-Web)，直接使用 Github 账号登录即可，记得在环境变量页填入 API Key；
3. 部署完毕后，即可开始使用；
4. （可选）[绑定自定义域名](https://vercel.com/docs/concepts/projects/domains/add-a-domain)：Vercel 分配的域名 DNS 在某些区域被污染了，绑定自定义域名即可直连。

## Get Started

1. Get [OpenAI API Key](https://platform.openai.com/account/api-keys);
2. Click
   [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Frandy7366%2FChatGPT-Next-Web&env=OPENAI_API_KEY&env=CODE&project-name=chatgpt-next-web&repository-name=ChatGPT-Next-Web);
3. Enjoy :)

## 保持更新 Keep Updated

如果你按照上述步骤一键部署了自己的项目，可能会发现总是提示“存在更新”的问题，这是由于 Vercel 会默认为你创建一个新项目而不是 fork 本项目，这会导致无法正确地检测更新。
推荐你按照下列步骤重新部署：

- 删除掉原先的 repo；
- fork 本项目；
- 前往 vercel 控制台，删除掉原先的 project，然后新建 project，选择你刚刚 fork 出来的项目重新进行部署即可；
- 在重新部署的过程中，请手动添加名为 `OPENAI_API_KEY` 的环境变量，并填入你的 api key 作为值。

本项目会持续更新，当你 Fork 项目之后，默认会每天自动同步上游代码，无需额外操作。

如果你想让手动立即更新，可以查看 [Github 的文档](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork) 了解如何让 fork 的项目与上游代码同步。
## 配置密码 Password

本项目提供有限的权限控制功能，请在 Vercel 项目控制面板的环境变量页增加名为 `CODE` 的环境变量，值为用英文逗号分隔的自定义密码：

```
code1,code2,code3
```

增加或修改该环境变量后，请**重新部署**项目使改动生效。

## 环境变量 Environment Variables

### `OPENAI_API_KEY` (required)

OpanAI 密钥。

Your openai api key.

### `CODE` (optional)

访问密码，可选，可以使用逗号隔开多个密码。

Access passsword, separated by comma.

### `BASE_URL` (optional)

> Default: `api.openai.com`

OpenAI 接口代理 URL。

Override openai api request base url.

### `PROTOCOL` (optional)

> Default: `https`

> Values: `http` | `https`

OpenAI 接口协议。

Override openai api request protocol.

## 开发 Development

点击下方按钮，开始二次开发：

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/randy7366/ChatGPT-Next-Web)

在开始写代码之前，需要在项目根目录新建一个 `.env.local` 文件，里面填入环境变量：


```
OPENAI_API_KEY=<your api key here>
```

### 本地开发 Local Development

> 如果你是中国大陆用户，不建议在本地进行开发，除非你能够独立解决 OpenAI API 本地代理问题。

1. 安装 nodejs 和 yarn，具体细节请询问 ChatGPT；
2. 执行 `yarn install && yarn dev` 即可。

### 本地部署 Local Deployment

```shell
bash <(curl -s https://raw.githubusercontent.com/randy7366/ChatGPT-Next-Web/main/scripts/setup.sh)
```


## 截图 Screenshots

![设置 Settings](./static/settings.png)

![更多展示 More](./static/more.png)
