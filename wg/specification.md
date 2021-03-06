# 写作规范

本文中指定了本书的写作规范与注意事项。

## 内容要求（必读）

写作前请认真规划自己的写作内容，想清楚自己要写什么，怎么写，列出提纲，再根据提纲逐步丰富内容。

要注意书籍写作和博客写作的区别。写博客以简练为主，可以用最简洁的文字描述问题即可。但书籍不同，需要有承上启下的段落，需要说清楚问题的来龙去脉，前因后果。说白了就是不能只写所以然，还要让读者知其所以然。

其次，注意所写主题的完整性。一上来就草草几句描述主题的方式不可取。可以参考三段论的方式思考写作内容：提出问题、分析问题、解决问题。另外，如果内容中出现专业术语，应对其进行解释说明（例如在写Istio的身份认证使用JWT方式，最好简单的解释JWT）。

严禁文档照搬或文档式的写法。文档式的内容就是只有骨架，没有血肉，无法成书。应该对内容加以润色和填充，让内容饱满易读，而不是枯燥乏味。照抄照搬官方文档的更不可取。

基于自己的理解进行写作（而不是文档的中文翻译）。如有可能，可以融入自己的技术价值观。书籍都是带有个人色彩的，是作者思想的结晶。读者希望能通过阅读和作者形成思想和想法的交换，否则直接去看官方文档即可。建议在写作前，认真吃透官方文档关于该主题的内容，然后用自己的语言简练的解释清楚即可。

### 书写禁忌

以下一些问题是首次写书的人容易犯的错误，在本书的写作过程中一定要避免出现。

- 文档式的写法：读上去像文档一样，只有骨架，没有血肉。
- 标题下缺少综述或介绍性质的段落：上来直接就写具体内容或操作步骤，缺少了承上启下的文字。
- 图表、代码正文没有说明：所有的图示、图表、代码都需要在正文中有说明性的文字。
- 操作步骤像流水账：对于实践性的内容，上来就写1、2、3步怎么做，没任何说明。步骤需要有一定说明，不仅仅是教怎么操作，还要解释为什么这样操作。
- 代码过多，缺乏解释：大篇幅的代码非常不友好，应按内容分开，并逐一解释。

## 注意事项

1. 请注意引用内容的版权，需标明出处；
1. 请不要发布涉及关于国家统一、宗教自由、民族相关的内容；
1. 请不要使用人像图片；
1. 请不要使用过分口语化或俚语表达；
1. 请勿在正文中引用带有具体公司名称的案例或评论；

## 文档组织规则

- 所有文档使用 markdown 格式撰写；
- 文中的图片请保存在本书的 GitHub 上；
- 图片必须给出标题；
- 所有引用的文章必须在文章底部的参考中给出链接，格式如 `title - domain.com`；
- 所有代码需要指明语言；

## 流程

1. 首先加入到本书的[协作群](https://github.com/servicemesher/istio-handbook/issues/42)
2. 在 [Issues](https://github.com/servicemesher/getting-started-with-knative/issues) 中认领你想要参与的章节（issue 标题为文章路径，内容填写标题和摘要）；
3. 一次最多同时认领 3 个 issue；
4. 由[编委会](editorial-board.md)成员审核后 merge 进 master 分支；
6. 合并后会立即发布到 <https://www.servicemesher.com/istio-handbook> 上；

## Header

每篇文章的头部都有一个使用 YAML 格式的 header，请在每次提交 PR 的时候填写，示例：

```yaml
authors: ["rootsongjc","malphi"]
reviewers: ["gorda","mathlsj"...]
```

**说明**

- authors：GitHub 账号，本文的主要作者，可以为一到两人；
- reviewers：GitHub 账号，只要修改过文章的人都是 reviewer；

## 排版规范

- 所有的英文跟中文之间要有一个空格；
- 参阅 [Istio 网站样式指南](https://istio.io/zh/about/contribute/style-guide/)；
- 专有名词中文译名参阅 <https://github.com/servicemesher/glossary>；
- 所有代码文件需要在 Markdown 格式中指明代码语言；
- 如果文中引用了外部参考资料，需要将参考资料的标题和链接放到文末的「参考」中；

## 图片规范

- 图片使用 PNG 或 JPG 格式；
- Markdown 中必须指明图片的标题，即格式为 `![title](path)`；
- 图片的 Markdown 文件中写的标题只需要表达图片本身的标题即可，不需要加序号；
- 图片中的文字描述使用中文，专业名词可以使用英文（为了出版需要）；
- 所有图片使用本地存储，放到 `images` 目录下，不需要在 `images` 目录下再创建子目录；
- 图片引用都使用相对路径；
- 图片文件名全为小写，使用英文命名，单词间使用连字符连接；
- 图片的分辨率不能太低（宽度最好不要低于 600 像素），保证文字清晰，没有水印，没有与要表达的信息无关的内容，例如签名、链接等；
- 引用的图片请注明引用来源（附上 URL）；
- 请勿使用人像照片；
- 图片配色得体大方；