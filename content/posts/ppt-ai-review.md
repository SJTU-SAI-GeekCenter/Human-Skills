---
title: "从逻辑到视觉：六款主流 PPT AI 工具深度横向测评"
date: 2024-05-20
description: "探索人、大模型与 PPT AI 的协同工作流，寻找最强的数字演示助手。"
tags: ["AI测评", "生产力", "SJTU-SAI"]
categories: ["技术分享"]
author: "罗梓宸, 陈秋实, 赵博"
showToc: true
TocOpen: true
---

# 主流 PPT AI 测评

## 前言

在数字时代，PPT 是我们不可或缺的演示工具，但传统制作方式不仅耗时费力，还容易遇到内容逻辑混乱、设计排版能力有限等困境。随着人工智能技术的飞速发展，PPT AI 工具应运而生，并逐步改变着 PPT 的创作方式。它们如同不知疲倦的“数字助理”，能够根据简单指令在几十秒内生成完整 PPT 初稿，不仅将人们从繁琐的重复劳动中解放出来，更重塑了生产力的范式。

现在，PPT AI 所具有的能力足以令人瞠目结舌。从智能配图、自动排版到语音转 PPT 功能，各类工具在不同维度展现独特优势。例如，一些工具能自动联网搜索高质量图片并融入幻灯片设计，而另一些则具备完备细致的修改功能，让用户能够对每一张 PPT 的方方面面进行优化调整。

但就目前来说，当用户使用 PPT AI 制作 PPT 时，我们认为 PPT AI 本质上仍然是在为用户提供一份“PPT 大纲”：将用户提供的文本大纲转换为包含视觉设计、时长控制等元素的可视化“PPT 大纲”。用一句话来概括，PPT AI 更像是用户的协作助手而非全自动的智能工具。

基于此认识，我们设计了本次测评的测评维度。在本文中，我们对领域内六个主流 PPT AI 工具进行了测评，并对其优缺点进行了分析，也进行了一些横向对比。对于各个 PPT AI 的缺点，我们也在文中提出了相应的解决方案。

此外，在本次测评中，我们尝试将大模型与 PPT AI 联合使用，通过三方共同构建工作流使 PPT 的创作更加便捷、准确，也一定程度解决了由提示词生成 PPT 所产生的稳定性降低问题，提高了可复现性。

---

## 测评方案介绍

### 1. 测评对象
本次测评共包含对以下六个 AI 工具的测试：
**WPS AI、Gamma、ChatPPT、Canva、Beautiful AI、AIPPT**

### 2. 测评背景与思路
此次测评所采用的方法主要基于我们在使用 AI 工具时的观察到的几个现象。目前市面上主流的 AI 工具的使用模式主要可以分为以下两种：
1. **提示词生成 PPT**：即用户提要求，AI 做 PPT。
2. **大纲生成 PPT**：即用户提供详细文件，AI 做 PPT。

**存在的问题：**
* 若使用提示词生成 PPT，容易导致细节描述不够清晰、完整，可复现性低等问题。
* 若使用大纲生成 PPT，用户需要提供详尽大纲。若手写大纲，可能费时费力，且因格式不符难以被 AI 工具识别。

因此，在本次测评中，我们使用 **大模型 + PPT AI 工具** 的方法，通过三方协作，尝试解决上述问题，使 PPT 的制作过程更加流畅。

### 3. 测评方法
我们可以借助大模型的语言理解能力，构建“**人——大模型——PPT AI 工具**”工作流，具体步骤如下（以 DeepSeek 大模型为例）：

#### （1）文字描述步骤
1. **设定角色**：用户先给大模型上传一个文档，给予大模型一个“人设”——PPT 大纲生成工作者。
2. **引导需求**：用户根据大模型的引导，写出（或修改）自己的要求。
3. **生成与优化大纲**：大模型生成大纲，用户将其粘贴至 PPT AI，并与 PPT AI 协作进行修改，注意要加入自己所需要的核心内容。
4. **生成 PPT**：用户将这一版大纲交给 PPT AI 工具生成 PPT。
5. **成品微调**：用户根据需要，调整 PPT 本身（若基本符合要求），或者调整大纲（若与设想有一定偏差）。
6. **循环迭代**：若调整大纲，则跳转至步骤 2 或步骤 3 的修改部分。

#### （2）流程图展示
![1图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/1.png)

### 4. 测评维度
此次，我们主要从以下三个大方向、五个方面对 PPT AI 工具进行测评：

1. **输出质量与稳定性**：输出的专业性、准确性和可靠性。
   * **设计**：整体视觉效果、排版等。
   * **文本**：文本与大纲的贴合度，文本合理程度等。
   * **配图**：配图准确性、贴合度，图像细节程度等。
2. **用户个性化要求的实现能力**
3. **调节与反馈能力**

# 一、对于领域内六个 PPT AI 工具的测评

## WPS AI 使用测评

### WPS AI 使用流程简述
0. 在 WPS 界面中点开“WPS AI”
1. 参照测评方案介绍部分，使用大模型生成大纲
2. 使用 WPS AIPPT 的“大纲生成 PPT”，将大模型生成的大纲粘贴至提示词区，AI 生成 PPT 内容
3. 用户选择模板
4. 生成 PPT

### 核心功能测评
**输出质量与稳定性：输出的专业性、准确性和可靠性。**

#### （1）视觉效果
整体视觉效果部分，由于是用户自己来选择模板，AI 工具的作用其实并不足够突出，但在挑选模板时，WPS AIPPT 会将更贴合用户大纲的 PPT 模板放在靠前的位置。就我们所用于测试的 5 个 demo 而言，使用两种方法生成 PPT 时，我们都能从 AI 推荐中挑选出具有优秀视觉效果的模板（下面是两个示例）：

![2图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/2.png)
![3图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/3.png)

在局部呈现上，WPS AI 仍显得不足。例如，在测评中，我们在大纲中加入“呈现形式：左侧 - 学习路径图：以时间轴形式展示‘大一上：入门项目 → 大一下：进阶项目 → 大二及以后：竞赛项目’”。这样对于局部的设计方案，最终得到的结果如下：

![4图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/4.png)

很显然不符合我们的要求，我们在后文对文本能力的测评中一并讨论这类问题。

#### （2）文本
文本部分，如果使用大纲生成 PPT 的方案，WPS AI 工具目前仍有不足，会出现大纲要求与实际生成 PPT 不一致的情况（如下图）：

![5图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/5.png)

概括来说，有如下两点问题：
* **WPS AI “大纲生成 PPT”功能会直接将用户所提供的“大纲”作为 PPT 正文的文本**：如果用户提供的大纲中没有提供具体的文本内容，那么 AI 会将大纲中内容以外的信息（如视觉效果设计、图示排版方案等）作为内容填充至文本框中。
* **内容排版上，对大纲本身所包含的信息量要求很高**：WPS AI 对于大纲当中所提到的要点具有一定的续写能力，但不能根据中心观点大量扩写。

#### （3）配图
由于 WPS AIPPT 主要是从网络上获取配图来源，如果用户希望配图能够包含具体含义（粗略一点如强调重点，具体一点如图表等），我们不建议使用 WPS AIPPT。在测试中，WPS AI 生成图片时，大纲意图的把握、图片内容生成的精细度等层面，都没有达到应用的标准。但如果用户只需要配图达到美观的效果，并不需要其承载实际含义的话，使用 PPT AI 配图往往是个便捷的选择。

### 2、用户个性化要求的实现能力

在本次测试的所有 demo 中，我们都加入了针对特定场景的要求，如：

> 【重点页面】零基础友好保障 (打消顾虑)
> 标题：零基础？这正是我们擅长的！
> 呈现形式：
> 左侧 - 学习路径图：以时间轴形式展示“大一上：入门项目 → 大一下：进阶项目 → 大二及以后：竞赛项目”。
> 右侧 - 支持体系：并列展示“系统化培训课程”、“一对一学长导师制”、“往届成功案例（如张同学）”。
> 口头话术：“去年的张同学，和你们一样带着好奇加入，现在已能独立带队项目。我们的体系就是为每一位新手设计的，你只需要带上热情和时间。”

所碰到的问题与 1 中所提到基本相同，我们不再赘述。但如果用户希望实现相对更加面向于内容的要求，如调整语气等，只要在大纲中加入相应的要求，WPS AI 就能够作出相应的调整。

### 3、调整与反馈能力

对于 1-（2）中所提到的文本生成问题，我们尝试仍用 WPS AI 内置的工具进行修改：我们使用“AI 生成单页”，将原大纲当中对应的部分直接输入，下面是修改后的结果：

![6图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/6.png)

对于 1-（1）中所提到的视觉效果问题， we 采用 WPS 内置的“美化助手”进行解决，效果如下：

![7图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/7.png)

WPS AI 对于两个问题的修改能力基本符合实际应用要求。

---

## Gamma 使用测评

### Gamma 使用流程简述
0. 登录 gamma.app（需要 vpn）
1. 参照测评方案介绍部分，使用大模型生成大纲
2. 使用 Gamma 的“使用 AI 创建——粘贴文本”，将大模型生成的大纲粘贴至提示词区，选择“根据笔记或者大纲生成”
3. 用户进行细节设置：文本内容及视觉效果
4. 生成 PPT

### 二、核心功能测评
**输出质量与稳定性：输出的专业性、准确性和可靠性。**

#### （1）视觉效果
整体视觉效果部分，Gamma 采用用户自行选择主题的方式，相较于选择模板而言，给予了 AI 工具更多的发挥空间，却也在理论上引入了更多不稳定性。Gamma 在对于文本框的排布、字体的大小等方面的表现略微不如 WPS AIPPT。在风格上，Gamma 所呈现的 PPT 更像是应用在学术类会议的报告 PPT ，大多偏简约风（下面是两个示例）：

![8图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/8.png)
![9图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/9.png)

在局部呈现上，Gamma 的表现相当出色。例如：在 WPS AIPPT 测评中， we 曾针对“路径图”的生成进行了讨论。在测评 Gamma 时，我们也同样向它抛出了这个难题，下面是 Gamma 的应对：

![10图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/10.png)
![11图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/11.png)
可以看到，Gamma 交出了一份令人满意的答卷。

#### （2）文本
与本次所测评的几个其它 PPT AI 工具相比，Gamma 的文本生成能力十分亮眼。在我们 5 份 demo 的测评中，Gamma 并没有出现其余所有 PPT AI 所出现的问题，如误读大纲，扩写能力不足等，下面仍然列出两个例子：

![12图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/12.png)
![13图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/13.png)

#### （3）配图
Gamma 的配图主要由内置模型生成。采用此方法生成的配图，往往在设计上会更加贴切，因为 AI 能够更好地根据 PPT 主题/模板的设计风格（色调、画风等）进行图片的创作，但其缺点仍在：AI 在把握大纲/文案对图片细节的要求时往往就更加容易出错。同样令人意外的是，Gamma 在对于配图的文案匹配度、配图细节（如文字）等的处理上也得心应手。

![14图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/14.png)

### 2、用户个性化要求的实现能力
也正如前文所述，对于用户在画面设计上的要求，Gamma 基本都能够从容地应对。在内容上，Gamma 也具备了极强的需求实现能力。不论是在大纲生成 PPT 阶段，还是 PPT 生成后的用户调整阶段，Gamma 都配置了丰富的工具库。

![15图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/15.png)
![16图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/16.png)

### 3、调整与反馈能力
Gamma 在用户交互层面考虑得很细致：在文本上，对于文本内容的问题，用户可直接与 Gamma 内置模型协作进行修改；对于文本分布、格式的问题，用户能够直接使用内置工具栏进行快速修改。

对于图片、表格的插入，Gamma 具有相当完备的功能。如果对 AI 自动匹配的图片不满意，用户可以通过点击图片，直接唤出搜索框/本地上传/AI 绘图进行调整。

![17图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/17.png)
![18图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/18.png)
此外，对于一些特殊的元素，如代码块、数学公式等，Gamma 都能直接支持，这也是 Gamma 在学术/技术类演示场景下的一大杀器。

---

## ChatPPT 使用测评

### 1、ChatPPT 使用流程简述
0. 网站：chat-ppt.com
1. 将提示词输入常用大模型软件（DeepSeek, 豆包等）生成初版大纲。
2. 将初版大纲粘贴至 ChatPPT 中，生成第二版大纲。
3. 与 ChatPPT 交互，修改第二版大纲。
4. 确定大纲，ChatPPT 开始生成 PPT。
5. 自行修改 PPT。

### 2、核心功能测评

#### （1）输出质量和稳定性：输出的专业性、准确性和可靠性

**① 风格设计**
在生成风格时，ChatPPT 会询问演讲场景和面向人群，以确认更加精细的要求，如下图：

![19图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/19.png)

**② 图片质量**
在生成图片时，有两种选择：其一是选择使用自己的图库，其二是 AI 生成。AI 生成有两种选择，一个是使用已经生成好的 AI 图库里的内容，另一个是 AI 实时绘图。其中 AI 实时绘图是需要 SVIP 才能使用，但这项功能在其他 PPT AI 类产品中大多是免费功能或基本功能。而且，生成的图片质量较差，图片中涉及文字生成时，往往会生成混乱的符号，有时图文并不相关。

![20图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/20.png)

至于其说到的使用 Nanobanana 进行绘图，似乎就更加让人失望了。

**③ 文本**
ChatPPT 在生成文本时，并不能正确区分大纲和需要生成的内容的区别，往往会把用户提出的具体要求，如“这段文字大约 2 分钟讲完”、“这段风格要活泼”等内容，直接呈现在 PPT 中。如下图：

![21图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/21.png)

此外，ChatPPT 生成的文本大多十分单薄，无法达到进行展示的要求，对于大纲中指出需要扩充的部分也未能进行扩充。所以，文本部分只能由用户自行补充完整。

#### 2. 用户个性化要求实现能力
在本次测试的所有 demo 中，我们都加入了个性化的特定场景，如在生成“社团” PPT 时，我们对其进行了细致的区分，将这一场景细分成了三个具体的情景（社团招新，重点社团申请，社团文化节宣传），并让 ChatPPT 制作了三份不同的 PPT。

在这方面，ChatPPT 的效果是不错的，可以精准地区分三个 PPT 的受众与场所不同带来的风格差别，这或许得益于在创建大纲时，ChatPPT 对用户进行的细致提问。但是，在内容生成方面，ChatPPT 依然不能识别要求和内容的区别，会把情境的不同直接展示在 PPT 上，让观感并不好。

此外，面对预设的情景，ChatPPT 也只会把情景写在 PPT 上，而不会委婉地展示，比如我们在其中一个 demo 中预设了专家的考核，而 ChatPPT 是这样解决的：

![22图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/22.png)

#### 3. 调节与反馈能力
在调节与反馈能力上，ChatPPT 的能力几乎等于 0，除了大纲可以进行修改，对后续的修改，ChatPPT 可以说是什么都做不到。这种做不到体现在两方面：

* **第一点，对指令不理解：**
![23图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/23.png)

* **第二点，无法正确地作出修改：**
![24图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/24.png)

总之，ChatPPT 这种半成品的感觉确实让人难以接受。这款产品并不适合用于直接生成 PPT，而更适合作为一种辅助设计的插件。

---

## Canva 使用测评

### 1、Canva 使用流程简述
0. 网站：canva.com
1. 参照测评方案介绍部分，使用大模型生成大纲
2. 登录 Canva，点击“创建设计”，搜索并进入“魔法设计 (Magic Design)”
3. 投喂大纲
4. 选择风格，生成 PPT

### 2、核心功能测评

#### （1）视觉效果
整体视觉偏现代/卡通/优美/简约，可在生成之前选择风格，列表如下：

![25图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/25.png)

同一个文件前后视觉风格能保持高度连贯，由于是较专业的设计软件，模板很丰富，色彩丰富，以鲜艳为主。

![26图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/26.png)
![27图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/27.png)
在局部设计上，Canva貌似并不擅长，很少见组件和图表，其所做的大部分是在模板背景上添加文本框和图片，部分局部设计仅限于下图的简单组件，且中文字体单一。

![28图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/28.png)

可见，Canva的设计倾向整体的风格一致，局部设计能力偏弱。

（2）文本生成
Canva AI能根据用户提示词生成一些简单小标题和句子，少见长段文字，在用户要求之后可以进行扩写，文字的质量不错。对于大纲中文字的要求，Canva AI则会进行一些简化。

![29图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/29.png)
![30图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/30.png)
相比于其他工具，基本不会出现把指令直接当作文案输入进去的情况，可见模型的总结能力还是不错的。

#### （3）配图
主要为 AI 生成和图库检索（会带有 Canva 水印），相关度尚可，生成的图片卡通风格更多些。

![31图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/31.png)

![32图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/32.png)

### 2、 用户个性化要求的实现能力
在本次测试的所有 demo 中，我们都加入了针对特定场景的要求，如：
【重点页面】零基础友好保障 (打消顾虑)
标题：零基础学习，完全可以实现
![33图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/33.png)
可见，我们的测评对象只是简单给标题篇配图，并没有突出的意味，在这项能力上明显是相对较弱的。


### 3、 调整与反馈能力
Canva AI 支持聊天交互，会主动确认部分细节，也支持在生成完成之后提出要求进行修改，不过这里的修改大部分时候是重新生成整个幻灯片，不支持单页面调整。通常其会生成两三套不同的设计供用户选择，并在生成后可以由用户自主在编辑页面使用各种图形设计工具，以弥补 AI 生成幻灯片设计缺乏的问题。
整体来说， Canva AI 智能化程度较高，模板丰富，不过乏于自动化设计和要点突出显示。

---

## Beautiful AI 试用测评

### 一、使用流程简述
0、 登录 beautiful . ai 网站（需使用 VPN ）->创建演示文稿-> Create With AI
1、 参照前言，使用 Deepseek 模型生成 PPT 大纲。
2、 输入生成好的提示词，等待生成大纲后进行交互确认，选择主题风格、图源（网络  /Beautiful 图库/ AI 生成）和语言。
3、 生成 PPT

### 二、核心功能测评
#### 1、 输出质量与稳定性：输出的专业性、准确性和可靠性
**（1）视觉效果**
整体色调以黑白为主，简约大气，质量稳定。供选择的 Theme 主要的区别在于色调冷暖和字体风格。页面间的设计连贯，动画流畅，让用户比较舒心。
![34图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/34.png)
![35图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/35.png)
![36图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/36.png)

在局部设计呈现方面， Beautiful . ai 能较合理地穿插使用各种设计元素，能把提示词里的设计要求大部分实现，也有部分不能准确识别，呈现下图的情况。
![37图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/37.png)

![38图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/38.png)

总体来说，视觉效果较好且通用。

**（2）文本生成**
文本部分，能基本分辨大模型生成大纲中的文案与指令，也难免会出现照抄“获奖趋势与奖项分布”“本页面是封面页”文本这种情况，文案自主编辑扩写能力一般，能自主完成小标题和短句的写作。更多时候， PPT 所包含的文案是占位指示性的，提出主旨引导用户自己编辑和改写，因此其职能倾向于让用户在其设计基础上进行文案的优化。

![39图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/39.png)

![40图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/40.png)
近期（2026年2月9日左右）， Beautiful . ai 迎来一次更新，原有的语言模块选择变得很少，且没有中文（以前基本支持所有语言），这一点对国内用户不是很友好。在提示词界面明确强烈要求使用中文制作，并将语言设为” Auto ”后仍有几率发生通篇或者部分页面使用英文的情况，差强人意。下图展示了中文PPT里夹杂的英文页面：


![41图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/41.png)

（3）配图
前文提到过，图源可选择网络、 AI 生成或自建库。网络图片的相关度和质量堪忧； AI 生成图片的质量和相关度都不错，只是囿于当前技术，图片汉语文字“鬼画符”的问题严重，与本工具的智能程度关系不大；自建库的图片则是比较精美的示例图，与内容关系不大了。
当然，对于正式场合的 PPT ，我们不建议使用 AI 或网络图片。仅限于美观，不要求携带信息量的话， AI 生成和图片库值得一试。

2、用户个性化要求的实现能力
在本次测评中，我们在每个 demo 里都加入了针对特定场景的要求，如：
【重点页面】零基础友好保障 (打消顾虑)

![42图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/42.png)
呈现形式：分模块呈现培训体系、学长辅导、成功案例。
不过从多个用例的测评看下来，个性化要求的实现能力不算突出，结合前面提到的中英文使用紊乱的情况可以看出，该工具在一定程度上淡化了用户强调的需求，而是通过公式化追求整体的一致性。

3、调整与反馈能力
目前， BeautifulAI 尚不支持在生成输出之后再一次通过提示词进行页面改动的功能。取而代之的是，它在生成之后每一页面都提供几张备选成片，并支持更改主题颜色、图文排版、播放动画等项目。
![43图](https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/43.png)
<div style="display: flex; flex-wrap: wrap; gap: 10px; justify-content: center;">
  <img src="https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/44.png?raw=true" width="30%" />
  <img src="https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/45.png?raw=true" width="30%" />
  <img src="https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/46.png?raw=true" width="30%" />
  <img src="https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/47.png?raw=true" width="30%" />
  <img src="https://github.com/claptrapp222/Human-Skills-1/blob/main/static/img/48.png?raw=true" width="30%" />
</div>
总之，该工具在设计上的能力较为出色，但在提示词处理、语言选择、调整反馈等方面依然有提升潜力，是一款不错的提升效率的设计工具。

### 二、核心功能测评

#### 1、输出质量和稳定性：输出的专业性、准确性和可靠性

**（1）风格设计**
在生成风格时， AIPPT 会参考大纲中的提示词，提供3个以上的模板风格供用户选择。 AIPPT 对于通过提示词来提供模板的能力是比较强的，可以根据同一大纲但情景不同提供出不同的模板。比如在宣传社团和社团招新这两个不同的情境，给出了两个较好的示范。


（社团招新）


（社团展示）

**（2）配图**
AIPPT 的配图方式有三种： AI 配图，网络配图和自行配图，在必要的情况下，用户往往会选择自行配图。但是为了测试 AIPPT 的性能，本次选择了 AI 配图。 AIPPT 的 AI 配图工作是由豆包完成的，效果仅仅能被称作勉强够用。在图片中涉及文字时效果会大打折扣， AI 的味道过于严重，让人一眼就能看出是 AI 生成的，但是文字生成的很清楚，并不会生成一堆符号，但文字的质量低下，大多是 PPT 内容的重复，如下图：



**（3）文本**
AIPPT 在生成文本时可以正确区分大纲中的要求和具体文本部分，并不会把要求原封不动的搬入 PPT 中。相比之下，市面上其他的 PPT AI 产品会把用户提供的大纲作为 PPT 正文的文本，即若用户没有对大纲中的某一部分做出具体的文本要求，其他产品会将无关信息作为内容直接填充进文本里。

#### 2、用户个性化要求的实现能力
在本次测试的所有 demo 中，我们都加入了个性化的特定场景，如在生成“社团” PPT 时，我们对其进行了细致的区分，将这一场景细分成了三个具体的情景（社团招新，重点社团申请，社团文化节宣传），并让 AIPPT 制作了三份不同的 PPT ，在这方面， AIPPT 的效果是不错的，可以精准的区分三个 PPT 的受众与场所不同带来的风格差别，但是，在具体文本的呈现上， AIPPT 并不能做出差异化的文本，大体只是将提供的基本信息复述了三遍。而且，文本的丰富能力较弱。如下图所示，很多文本仅仅生成一句话，甚至不能够被称为文本。



#### 3、调节与反馈能力
在调节与反馈能力上， AIPPT 做得就没有那么令人满意了。首先是，网页版的 AIPPT 并不能支持单页 PPT 的调节，当 PPT 生成结束后，若想修改必须自己修改。其次，仅仅可以通过修改 AIPPT 生成的大纲来修改 PPT ，无法更加具体地修改。更为难以使用的是，无法保留对话，若在 PPT 生成结束后想再次对 PPT 进行修改，仅仅能自行修改或者重复生成 PPT 时的操作，这一点，让完善 PPT 的工作变得格外繁琐。










---

## AIPPT 测评

### 一、 AIPPT 使用流程
0、进入 AIPPT 官网 www . aippt . cn
1、将提示词输入常用大模型软件（ ds ,豆包等）生成初版大纲
2、将初版大纲粘贴至 AIPPT 中，生成第二版大纲
3、与 AIPPT 交互，修改第二版大纲
4、确定大纲， AIPPT 开始生成 PPT
5、自行修改 PPT







### 附件下载
本文测评所使用的 AI 人设指令集已整理为文档，欢迎下载参考：

[点击下载：附件：AI人设——做ppt.docx](https://github.com/claptrapp222/Human-Skills/blob/main/static/附件：AI人设——做ppt.docx)
*本文由 SJTU-SAI GeekCenter 成员测评产出。*
