# 风格指南与检查器

风格指南一般凝练了整个技术写作团队的多年的精华，成熟的风格指南可以让技术作家快速熟悉团队遣词造句以及行文风格的要求，确保内容的一致性。在做技术文档写作的时候，成熟的团队都有有自己的风格指南(style guide)。



## 风格

在讲解风格指南之前，我们先说一说风格，因为有了风格才需要有指南。

假设有两个人：甲和乙进入咖啡厅点咖啡，他们分别是这样点咖啡的：

甲

> Small Coffee
>
> Extra light, no sugar. 
>
> I'm in a rush.

乙

>Hi, Cynthia. Can I get
>
>A small coffee, 
>
>Extra light, no sugar?
>
>Thanks.



甲显得比较莽撞，听起来就比较忙，也很不耐烦，而乙则会让人觉得比较体贴，不着急，而且比较友好。语言是思想的外衣，不同的表达方式，会让听众形成不同的观感。



再以GE和MINI汽车为例，因为历史和品牌定位的不同，两个品牌有了自己的风格。



|      | GE                                                           | MINI                                                         |
| ---- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 风格 | - imaginative <br />- responsible<br /> - inspirational      | - Confident <br />- Joyful <br />- Rebellious                |
| 文案 | Ge works hard to make house a home. <br />We're determined to solve the world's biggest problems. | You know that the dream you have. <br />But in the vent of a late-night flat tire or wild armadillo attack |

GE的信条是“imagination at work"，他们总是想让世界知道，GE每天的工作会让整个世界收益。正是以为你这个目的，我们可以感觉到他们的文案也是想让受众觉得他们的业务非常重要。

MNI的人群定位是有生活的幽默感，反对世俗，想开心生活，所以文案上也能看出来这一点。

因为个性所以有了自己的风格，而风格又会影响一个人的讲话的方式。



## 微软风格

不仅消费者公司有调性，其实高科技公司也有自己的调性。例如微软公司希望用户能感受到微软是：inspirational, responsible, empathetic, polite, supportive and encouraging，为了达到这个效果，微软也制定了具体的细则来指导工程师的写作。

### inspirational

要求：强调用户可以做哪些事情，而不是不能做哪些。鼓励用户是帮助用户实现潜能的重要组成部分，帮助用户解决问题，但是如果能有机会让用户尝试之前没有想到的功能也是非常好的。

> You can add a personal touch to your computer by changing the computer's theme, color, sounds, desktop background, screen saver, font size, and user account picture.



### Responsible

我们的责任不仅仅是一个伟大产品的公司，我们还应该思考用户会如何看待我们的评价。

>Microsoft style
>
>Free technical support is available when you register with Microsoft.

>Non Microsoft style
>
>You must register with Microsoft to received free technical support.



### Polite

不应该让用户觉得被冒犯，或者甲方高高在上。



>Microsoft style
>
>The file is protected and can't be deleted without specific permission.

>Not Microsoft style
>
>Can't delete New Text Document: Access is denied.



更多内容，大家可以参见 [Microsoft Manual of Style](https://www.amazon.com/Microsoft-Manual-Style-4th-Corporation/dp/0735648719/ref=sr_1_1?keywords=Microsoft+Manual+of+Style&qid=1639042143&sr=8-1)



## 风格指南

常见的风格指南：

- [Microsoft Style Guide](https://docs.microsoft.com/en-us/style-guide/welcome/)
- [Google Documentation Style Guide](https://developers.google.com/style/)
- [18F Content Guide](https://content-guide.18f.gov/our-style/)
- [Apple Style Guide](https://books.apple.com/us/book/apple-style-guide/id1161855204)





## Linter

风格指南一般需要搭配检查器共同工作，否则完全靠写作者的记忆，压力较大而且容易出错。

开发者在写代码的时候，常常需要依赖 **Linter**查找错误、冲突或代码风格等问题。在Docs as Code的开发模式中，也常常将文本当成代码来进行检查。

常见Linter

- [alex](https://alexjs.com/)
- [Vale](https://github.com/errata-ai) | [vale-vscode](https://github.com/errata-ai/vale-vscode)
- proselint
- [languagetool](https://languagetool.org/)







可检查的规则

- [Vale 的 *Microsoft Writing Style Guide* 的检查规则](https://github.com/errata-ai/Microsoft)