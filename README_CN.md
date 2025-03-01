![](./images/describe-cn.jpg)
<p align="center">
  <a href="./README.md">English</a> |
  <a href="./README_CN.md">简体中文</a> |
  <a href="./README_JA.md">日本語</a> |
  <a href="./README_ES.md">Español</a>
</p>


[官方网站](https://dify.ai) • [文档](https://docs.dify.ai/v/zh-hans) • [Twitter](https://twitter.com/dify_ai) •  [Discord](https://discord.gg/FngNHpbcY7)

**Dify** 是一个易用的 LLMOps 平台，旨在让更多人可以创建可持续运营的原生 AI 应用。Dify 提供多种类型应用的可视化编排，应用可开箱即用，也能以“后端即服务”的 API 提供服务。

通过 Dify 创建的应用包含了：

- 开箱即用的的 Web 站点，支持表单模式和聊天对话模式
- 一套 API 即可包含插件、上下文增强等能力，替你省下了后端代码的编写工作
- 可视化的对应用进行数据分析，查阅日志或进行标注

Dify 兼容 Langchain，这意味着我们将逐步支持多种 LLMs ，目前支持的模型供应商：

* **OpenAI**：GPT4、GPT3.5-turbo、GPT3.5-turbo-16k、text-davinci-003 

* **Azure OpenAI Service**
* **Anthropic**：Claude2、Claude-instant

> 我们为所有注册云端版的用户免费提供了 1000 次 Claude 模型的消息调用额度，登录 [dify.ai](https://cloud.dify.ai) 即可使用。

* **Hugging Face Hub**（即将推出）

## 使用云服务

访问 [Dify.ai](https://cloud.dify.ai)

## 安装社区版

### 系统要求

在安装 Dify 之前，请确保您的机器满足以下最低系统要求：

- CPU >= 1 Core
- RAM >= 4GB

### 快速启动

启动 Dify 服务器的最简单方法是运行我们的 [docker-compose.yml](docker/docker-compose.yaml) 文件。在运行安装命令之前，请确保您的机器上安装了 [Docker](https://docs.docker.com/get-docker/) 和 [Docker Compose](https://docs.docker.com/compose/install/)：

```bash
cd docker
docker compose up -d
```

运行后，可以在浏览器上访问 [http://localhost/install](http://localhost/install) 进入 Dify 控制台并开始初始化安装操作。

### Helm Chart

非常感谢 @BorisPolonsky 为我们提供了一个 [Helm Chart](https://helm.sh/) 版本，可以在 Kubernetes 上部署 Dify。
您可以前往 https://github.com/BorisPolonsky/dify-helm 来获取部署信息。

### 配置

需要自定义配置，请参考我们的 [docker-compose.yml](docker/docker-compose.yaml) 文件中的注释，并手动设置环境配置，修改完毕后，请再次执行 `docker-compose up -d`。

## Roadmap

我们正在开发中的功能：

- **数据集**，支持更多的数据集，例如同步 Notion 或网页的内容
我们将支持更多的数据集，包括文本、网页，甚至 Notion 内容。用户可以根据自己的数据源构建 AI 应用程序。
- **插件**，推出符合 ChatGPT 标准的插件，或使用 Dify 产生的插件
我们将发布符合 ChatGPT 标准的插件，或者 Dify 自己的插件，以在应用程序中启用更多功能。
- **开源模型**，例如采用 Llama 作为模型提供者，或进行进一步的微调
我们将与优秀的开源模型如 Llama 合作，通过在我们的平台中提供它们作为模型选项，或使用它们进行进一步的微调。

## Q&A

**Q: 我能用 Dify 做什么？**

A: Dify 是一个简单且能力丰富的 LLM 开发和运营工具。你可以用它搭建商用级应用，个人助理。如果你想自己开发应用，Dify 也能为你省下接入 OpenAI 的后端工作，使用我们逐步提供的可视化运营能力，你可以持续的改进和训练你的 GPT 模型。

**Q: 如何使用 Dify “训练”自己的模型？**

A: 一个有价值的应用由 Prompt Engineering、上下文增强和 Fine-tune 三个环节组成。我们创造了一种 Prompt 结合编程语言的 Hybrid 编程方式（类似一个模版引擎），你可以轻松的完成长文本嵌入，或抓取用户输入的一个 Youtube 视频的字幕——这些都将作为上下文提交给 LLMs 进行计算。我们十分注重应用的可运营性，你的用户在使用 App 期间产生的数据，可进行分析、标记和持续训练。以上环节如果没有好的工具支持，可能会消耗你大量的时间。

**Q: 如果要创建一个自己的应用，我需要准备什么？**

A: 我们假定你已经有了 OpenAI API Key，如果没有请去注册一个。如果你已经有了一些内容可以作为训练上下文，就太好了。

**Q: 提供哪些界面语言？**

A: 现已支持英文与中文，你可以为我们贡献语言包。

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=langgenius/dify&type=Date)](https://star-history.com/#langgenius/dify&Date)


## 贡献

我们欢迎你为 Dify 作出贡献帮助 Dify 变得更好。我们欢迎各种方式的贡献，提交代码、问题、新想法、或者分享你基于 Dify 创建出的各种有趣有用的 AI 应用。同时，我们也欢迎你在不同的活动、研讨会、社交媒体上分享 Dify。

### 贡献代码
为了确保正确审查，所有代码贡献 - 包括来自具有直接提交更改权限的贡献者 - 都必须提交 PR 请求并在合并分支之前得到核心开发人员的批准。

我们欢迎所有人提交 PR！如果您愿意提供帮助，可以在 [贡献指南](CONTRIBUTING_CN.md) 中了解有关如何为项目做出代码贡献的更多信息。

### 提交问题或想法
你可以通过 Dify 代码仓库新增 issues 来提交你的问题或想法。如遇到问题，请尽可能描述你遇到问题的操作步骤，以便我们更好地发现它。如果你对我们的产品有任何新想法，也欢迎向我们反馈，请尽可能多地分享你的见解，以便我们在社区中获得更多反馈和进一步讨论。

### 分享你的应用
我们鼓励所有社区成员分享他们基于 Dify 创造出的 AI 应用，它们可以是应用于不同情景或不同用户，这将有助于为希望基于 AI 能力创造的人们提供强大灵感！你可以通过 [Dify-user-case 仓库项目提交 issue](https://github.com/langgenius/dify-user-case) 来分享你的应用案例。

### 向别人分享 Dify
我们鼓励社区贡献者们积极展示你使用 Dify 的不同角度。你可以通过线下研讨会、博客或社交媒体上谈论或分享你使用 Dify 的任意功能，相信你独特的使用分享会给别人带来非常大的帮助！如果你需要任何指导帮助，欢迎联系我们 support@dify.ai ,你也可以在 twitter @Dify.AI 或在 [Discord 社区](https://discord.gg/FngNHpbcY7)交流来帮助你传播信息。

### 帮助别人
你还可以在 Discord、GitHub issues或其他社交平台上帮助需要帮助的人，指导别人解决使用过程中遇到的问题和分享使用经验。这也是个非常了不起的贡献！如果你希望成为 Dify 社区的维护者，请通过[Discord 社区](https://discord.gg/FngNHpbcY7) 联系官方团队或邮件联系我们 support@dify.ai.


## 联系我们

如果您有任何问题、建议或合作意向，欢迎通过以下方式联系我们：

- 在我们的 [GitHub Repo](https://github.com/langgenius/dify) 上提交 Issue 或 PR
- 在我们的 [Discord 社区](https://discord.gg/FngNHpbcY7) 上加入讨论
- 发送邮件至 hello@dify.ai

## 安全

为了保护您的隐私，请避免在 GitHub 上发布安全问题。发送问题至 security@dify.ai，我们将为您做更细致的解答。

## Citation

本软件使用了以下开源软件：

- Chase, H. (2022). LangChain [Computer software]. https://github.com/hwchase17/langchain
- Liu, J. (2022). LlamaIndex [Computer software]. doi: 10.5281/zenodo.1234.

更多信息，请参考相应软件的官方网站或许可证文本。

## License

本仓库遵循 [Dify Open Source License](LICENSE) 开源协议。
