从今天开始，开发人员可以开始使用 DALL·E API 构建应用程序。

开发人员现在可以通过我们的 API 将DALL·E直接集成到他们的应用程序和产品中。超过 300 万人已经在使用 DALL·E 来扩展他们的创造力并加快他们的工作流程，每天生成超过 400 万张图像。开发人员可以在几分钟内开始使用相同的技术进行构建。

```
#generations
curl https://api.openai.com/v1/images/generations \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer $OPENAI_API_KEY" \
  -d '{
    "prompt": "a photo of a happy corgi puppy sitting and facing forward, studio light, longshot",
    "n":1,
    "size":"1024x1024"
   }'

```

```
#edits
curl https://api.openai.com/v1/images/edits \
  -H "Authorization: Bearer $OPENAI_API_KEY" \
  -F image="@/Users/openai/happy_corgi.png" \
  -F mask="@/Users/openai/mask.png" \
  -F prompt="a photo of a happy corgi puppy with fancy sunglasses on sitting and facing forward, studio light, longshot" \
  -F n=1 \
  -F size="1024x1024"
```

```
#variations
curl https://api.openai.com/v1/images/variations \
  -H "Authorization: Bearer $OPENAI_API_KEY" \
  -F image="@/Users/openai/corgi_with_sunglasses.png" \
  -F n=4 \
  -F size="1024x1024"
```

![image](https://user-images.githubusercontent.com/13504729/216574134-d69dbc0c-0e13-4dad-bb07-d8c95e5fc685.png)

最先进的图像生成
DALL·E 的灵活性允许用户创建和编辑从艺术到逼真的原始图像。DALL·E擅长遵循自然语言描述，让用户可以清楚地描述他们想看到的内容。随着我们研究的发展，我们将继续将最先进的技术引入 API，包括图像质量、延迟、可扩展性和可用性方面的进步。

内置审核
结合我们在将 DALL·E 部署到全球 300 万艺术家和用户时吸取的信任和安全经验教训，开发人员可以放心地交付，因为他们知道内置的缓解措施（例如针对仇恨符号和血腥的过滤器）将处理节制的挑战性方面. 作为 OpenAI 负责任部署承诺的一部分，我们将继续将信任和安全放在首位，以便开发人员可以专注于构建。

DALL·E应用
我们与一些早期客户密切合作，他们已经在各种用例中将 DALL·E 构建到他们的应用程序和产品中。

微软将 DALL·E 引入一款名为Designer的全新图形设计应用程序，该应用程序可帮助用户创建专业品质的社交媒体帖子、邀请函、数字明信片、图形等。

微软还将 Bing 和 Microsoft Edge 中的 DALL·E 与 Image Creator 集成在一起，允许用户在网络结果未返回他们正在寻找的内容时创建图像。

CALA是世界上第一个时尚和生活方式操作系统。CALA 将整个设计流程——从产品构思一直到电子商务支持和订单履行——统一到一个数字平台中。在 DALL·E 的支持下，CALA 的新人工智能工具将允许用户从自然文本描述或上传的参考图像中生成新的设计理念。

Mixtiles是一家发展迅速的照片创业公司。他们使用软件和简单的悬挂体验来帮助数百万人创建漂亮的照片墙。Mixtiles 使用 DALL·E API 来创建和构建能引起情感共鸣的艺术品，通过引导用户完成捕捉童年记忆、梦想目的地等的创作过程。

我们很高兴看到我们的客户将使用 DALL·E 做什么，以及他们会想出什么创意。

使用 OpenAI 强大的模型进行构建
DALL·E在我们的 API 平台中加入了GPT-3、Embeddings和Codex，添加了一个新的构建块，开发人员可以使用它来创建新颖的体验和应用程序。所有 API 客户现在都可以使用 DALL·E API。
