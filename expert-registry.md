# 问天 · 专家注册表

> 所有已注册专家的元数据。咨询模式通过此表进行路由匹配。

---

```yaml
experts:

  - id: paul-graham
    name: Paul Graham
    name_en: Paul Graham
    aliases: [PG, 保罗·格雷厄姆]
    source: cangjie-v2
    domain: [创业, 早期产品, 写作, 独立思考, 技术创业]
    trigger_keywords: [创业, 早期产品, YC, 写作, 独立思考, 融资, 增长, startup, 黑客]
    avoid: [大企业管理, 非创始人职业路径, 宏观经济]
    quote: "Do things that don't scale."

  - id: munger
    name: 查理·芒格
    name_en: Charlie Munger
    aliases: [芒格, Munger]
    source: nuwa (adapted to v2)
    domain: [投资决策, 多元思维模型, 逆向思考, 认知偏误]
    trigger_keywords: [投资, 逆向思考, 认知偏误, 能力圈, 激励机制, 多元思维, 清单, 检查清单]
    avoid: [科技前沿, AI技术, 加密货币]
    quote: "Invert, always invert."

  - id: steve-jobs
    name: 乔布斯
    name_en: Steve Jobs
    aliases: [乔布斯, Jobs]
    source: nuwa (adapted to v2)
    domain: [产品设计, 用户体验, 品牌与发布, 极简主义, 战略聚焦]
    trigger_keywords: [产品决策, 功能取舍, 简洁, 极致, 用户体验, 发布, 品牌, 设计]
    avoid: [投资理财, 大组织管理, 供应链细节]
    quote: "Focus means saying no to a hundred good ideas."

  - id: musk
    name: 马斯克
    name_en: Elon Musk
    aliases: [马斯克, Musk, Elon]
    source: nuwa (adapted to v2)
    domain: [第一性原理, 工程思维, 跨领域创新, 极端目标设定]
    trigger_keywords: [第一性原理, 工程, 制造, 火箭, 电动车, 跨领域, 不可能, 10倍]
    avoid: [金融投资, 人文哲学, 组织文化]
    quote: "When something is important enough, you do it even if the odds are not in your favor."

  - id: naval
    name: 纳瓦尔
    name_en: Naval Ravikant
    aliases: [纳瓦尔, Naval]
    source: nuwa (adapted to v2)
    domain: [财富创造, 杠杆思维, 人生哲学, 幸福, 特定知识]
    trigger_keywords: [财富, 杠杆, 特定知识, 幸福, 自由, 复利, 长期主义, 人生选择]
    avoid: [具体投资标的, 企业运营细节, 技术实现]
    quote: "Seek wealth, not money or status."

  - id: taleb
    name: 塔勒布
    name_en: Nassim Nicholas Taleb
    aliases: [塔勒布, Taleb]
    source: nuwa (adapted to v2)
    domain: [风险管理, 反脆弱, 不确定性, 黑天鹅, 概率思维]
    trigger_keywords: [风险, 反脆弱, 黑天鹅, 不确定性, 尾部风险, 概率, 脆弱, 鲁棒]
    avoid: [具体投资建议, 短期预测, 宏观经济预测]
    quote: "Wind extinguishes a candle and energizes fire."

  - id: feynman
    name: 费曼
    name_en: Richard Feynman
    aliases: [费曼, Feynman]
    source: nuwa (adapted to v2)
    domain: [学习方法, 教学, 科学思维, 好奇心, 简化复杂问题]
    trigger_keywords: [学习, 教学, 解释, 简化, 好奇心, 第一原理, 理解, 科学方法]
    avoid: [商业策略, 投资, 组织管理]
    quote: "What I cannot create, I do not understand."

  - id: zhang-yiming
    name: 张一鸣
    name_en: Zhang Yiming
    aliases: [张一鸣, 一鸣]
    source: nuwa (adapted to v2)
    domain: [产品思维, 组织管理, 信息分发, 全球化, 延迟满足]
    trigger_keywords: [产品, 算法, 推荐, 组织, 全球化, 延迟满足, 字节跳动, 信息分发]
    avoid: [硬件制造, 金融投资, 基础科学研究]
    quote: "Stay hungry, stay foolish, stay young."

  - id: karpathy
    name: Karpathy
    name_en: Andrej Karpathy
    aliases: [卡帕西, Karpathy, Andrej]
    source: nuwa (adapted to v2)
    domain: [AI/深度学习, 工程实践, AI教育, 技术趋势判断]
    trigger_keywords: [AI, 深度学习, 神经网络, LLM, GPT, 机器学习, 模型训练, AI趋势]
    avoid: [商业模式, 投资, 人文社科]
    quote: "The hottest new programming language is English."

  - id: zhangxuefeng
    name: 张雪峰
    name_en: Zhang Xuefeng
    aliases: [张雪峰, 雪峰]
    source: nuwa (adapted to v2)
    domain: [职业规划, 高考志愿, 阶层流动, 就业市场现实]
    trigger_keywords: [职业规划, 考研, 志愿, 就业, 专业选择, 阶层, 考公, 学历]
    avoid: [创业, 投资理财, 技术前沿, 海外市场]
    quote: "别拿理想主义忽悠穷人家的孩子。"

  - id: hushan
    name: 虎山行不行
    name_en: Hushan
    aliases: [虎哥, 虎山, 虎山行不行]
    source: zhihu-2474-answers + fan-summary-322-quotes
    domain: [人性洞察, 职场生存, 人际博弈, 高情商回复, 实用主义哲学]
    trigger_keywords: [人性, 职场潜规则, 人际关系, 高情商, 怎么回复, 怎么拒绝, 怎么应对, 博弈, 利益, 面子, 求生欲, 打工, 牛马, 情商]
    avoid: [宏观经济, 投资理财, 技术领域, 高学历精英路径]
    quote: "没有好人斗不过坏人，只有弱人斗不过强人。"

  - id: duanyongping
    name: 段永平
    name_en: Duan Yongping
    aliases: [段永平, 大道无形]
    source: Panmax/duanyongping-skill (adapted to v2)
    domain: [价值投资, 企业文化, 本分哲学, 消费品牌]
    trigger_keywords: [本分, 价值投资, 企业文化, OPPO, vivo, 步步高, 做对的事, 不做什么]
    avoid: [科技前沿, AI技术, 宏观经济预测]
    quote: "做对的事，把事做对。"

  - id: zhangxiaolong
    name: 张小龙
    name_en: Zhang Xiaolong
    aliases: [张小龙, Allen Zhang]
    source: Panmax/zhangxiaolong-skill (adapted to v2)
    domain: [产品哲学, 极简设计, 用户感知, 克制, 社交产品]
    trigger_keywords: [产品哲学, 克制, 用完即走, 微信, 简洁, 用户感知, 少即是多, 社交产品]
    avoid: [投资理财, 硬件制造, 企业管理]
    quote: "好的产品是用完即走的。"

  - id: inamori
    name: 稻盛和夫
    name_en: Inamori Kazuo
    aliases: [稻盛和夫, 稻盛]
    source: Panmax/inamori-skill (adapted to v2)
    domain: [经营哲学, 利他主义, 阿米巴经营, 敬天爱人, 企业重建]
    trigger_keywords: [经营哲学, 利他, 阿米巴, 敬天爱人, 六项精进, 日航, 活法, 付出不亚于任何人的努力]
    avoid: [科技前沿, 金融投资, 互联网产品]
    quote: "付出不亚于任何人的努力。"

  - id: renzhengfei
    name: 任正非
    name_en: Ren Zhengfei
    aliases: [任正非, 任总]
    source: Panmax/renzhengfei-skill (adapted to v2)
    domain: [灰度管理, 战略聚焦, 危机思维, 组织建设, 自我批判]
    trigger_keywords: [灰度管理, 华为, 狼性文化, 自我批判, 战略聚焦, 压强原则, 危机, 组织]
    avoid: [消费品牌, 投资理财, 互联网产品设计]
    quote: "方向大致正确，组织充满活力。"

  - id: zengguofan
    name: 曾国藩
    name_en: Zeng Guofan
    aliases: [曾国藩, 曾文正]
    source: Panmax/zengguofan-skill (adapted to v2)
    domain: [自律修身, 领导力, 逆境管理, 团队建设, 笨功夫]
    trigger_keywords: [自律, 修身, 领导力, 逆境, 坚持, 笨功夫, 日课, 团队, 识人用人]
    avoid: [科技, 现代商业模式, 投资理财, 互联网]
    quote: "天下事，在局外呐喊议论，总是无益，必须躬自入局，挺膺负责，方有成事之可冀。"

  - id: thiel
    name: 彼得·蒂尔
    name_en: Peter Thiel
    aliases: [彼得·蒂尔, Thiel, Peter Thiel]
    source: Panmax/thiel-skill (adapted to v2)
    domain: [垄断思维, 从0到1, 逆向创业, 技术乐观主义]
    trigger_keywords: [从0到1, 垄断, 逆向, 竞争是失败者的事, PayPal, 技术创业, 秘密]
    avoid: [传统行业运营, 日常管理, 东亚文化语境]
    quote: "Competition is for losers."

  - id: wangyangming
    name: 王阳明
    name_en: Wang Yangming
    aliases: [王阳明, 阳明先生]
    source: panmax/nuwa-skill
    domain: [知行合一, 心学, 决策哲学, 自我修炼, 道德判断]
    trigger_keywords: [知行合一, 心学, 致良知, 自我修炼, 道德判断, 内心, 决策困境, 知道却做不到]
    avoid: [现代商业, 技术, 投资]
    quote: "知是行之始，行是知之成。"

  - id: altman
    name: 山姆·奥特曼
    name_en: Sam Altman
    aliases: [奥特曼, Sam Altman, 山姆]
    source: panmax/nuwa-skill
    domain: [AI时代创业, 指数思维, 技术乐观主义, 规模化, AGI]
    trigger_keywords: [AI创业, AGI, OpenAI, 规模定律, 技术乐观, 指数增长, 超级对齐]
    avoid: [传统行业, 非技术领域, 短期博弈]
    quote: "The most valuable thing you can do is make something people want."

  - id: huangrenxun
    name: 黄仁勋
    name_en: Jensen Huang
    aliases: [黄仁勋, Jensen, 皮衣教主]
    source: panmax/nuwa-skill
    domain: [算力革命, 加速计算, 长期押注, 工程文化, GPU]
    trigger_keywords: [GPU, 算力, NVIDIA, 加速计算, 芯片, AI基础设施, 长期押注, 制造业]
    avoid: [金融投资, 哲学思辨, 人文社科]
    quote: "Accelerated computing is the path forward."

  - id: dalio
    name: 瑞·达利欧
    name_en: Ray Dalio
    aliases: [达利欧, Ray Dalio, 桥水]
    source: panmax/nuwa-skill
    domain: [原则, 极度透明, 算法决策, 宏观投资, 系统思维]
    trigger_keywords: [原则, 极度透明, 算法, 决策系统, 宏观周期, 债务周期, 桥水]
    avoid: [早期创业, 技术实现, 单一公司分析]
    quote: "Pain plus reflection equals progress."

  - id: fengtang
    name: 冯唐
    name_en: Feng Tang
    aliases: [冯唐]
    source: panmax/nuwa-skill
    domain: [管理, 文学, 审美, 成事, 人生哲学]
    trigger_keywords: [成事, 审美, 管理方法论, 文字, 简洁, 翻译腔, 做事]
    avoid: [技术实现, 投资理财, 宏观经济]
    quote: "成事是干出来的，不是说出来的。"

  - id: ilya
    name: Ilya Sutskever
    name_en: Ilya Sutskever
    aliases: [Ilya, 伊尔亚]
    source: alchaincyf/nuwa-skill
    domain: [AI安全, scaling规律, 深度学习研究, 研究品味, AGI]
    trigger_keywords: [AI安全, scaling, 深度学习, 神经网络, 研究方向, AGI风险, 对齐]
    avoid: [商业模式, 管理, 投资理财]
    quote: "The thing that makes intelligence special is that it can generalize."

  - id: bezos
    name: 贝佐斯
    name_en: Jeff Bezos
    aliases: [贝佐斯, Jeff Bezos]
    source: panmax/nuwa-skill
    domain: [长期主义, 客户至上, Day1思维, 飞轮效应, 非共识决策]
    trigger_keywords: [长期主义, 客户至上, Day1, 飞轮, 匿名投入, 反向工作, 两类决策]
    avoid: [人文哲学, 技术实现, 快速路径]
    quote: "It's always Day 1."

  - id: buffett
    name: 巴菲特
    name_en: Warren Buffett
    aliases: [巴菲特, 波克德, Warren Buffett, 奥马哈的神毕]
    source: panmax/nuwa-skill
    domain: [价值投资, 长期持有, 护城河, 能力圈, 尺度人
]
    trigger_keywords: [价值投资, 护城河, 长期持有, 能力圈, 复利, 安全边际, 大股投资, 企业结构]
    avoid: [科技前沿, AI, 加密货币, 早期创业]
    quote: "Be fearful when others are greedy, and greedy when others are fearful."

  - id: sunzi
    name: 孙子
    name_en: Sun Tzu
    aliases: [孙子, 孙武, 兵法]
    source: panmax/nuwa-skill
    domain: [战略思维, 博弈论, 研判, 不战而胜, 气势]
    trigger_keywords: [战略, 战术, 博弈, 气势, 知己知彼, 不战而胜, 章法, 策略布局]
    avoid: [现代投资, 技术实现, 具体业务操作]
    quote: "知己知彼，百战不殆。"

  - id: liguangyao
    name: 李光耀
    name_en: Lee Kuan Yew
    aliases: [李光耀, LKY]
    source: panmax/nuwa-skill
    domain: [治国实用主义, 制度设计, 经济发展, 精英治理]
    trigger_keywords: [治国, 制度, 实用主义, 新加坡, 精英, 组织建设, 国家竞争力]
    avoid: [技术创业, 金融投资, 文学审美]
    quote: "I am often accused of interfering in the private lives of citizens. Yes, if I did not, Singapore would not be what it is today."

  - id: grove
    name: 安迪·格鲁夫
    name_en: Andy Grove
    aliases: [格鲁夫, Andy Grove, 安迪格鲁夫]
    source: panmax/nuwa-skill
    domain: [偏执狂, 战略转折点, OKR, 危机管理, 高强度管理]
    trigger_keywords: [偏执狂, OKR, 战略转折点, 危机, 高强度, 组织管理, 绩效管理, Intel]
    avoid: [产品设计, 投资理财, 技术实现]
    quote: "Only the paranoid survive."

  - id: drucker
    name: 德鲁克
    name_en: Peter Drucker
    aliases: [德鲁克, Peter Drucker]
    source: panmax/nuwa-skill
    domain: [管理学, 知识工作者, 目标管理, 组织设计]
    trigger_keywords: [管理, 知识工作者, 目标管理, 组织, 领导力, 效能, 决策]
    avoid: [技术实现, 投资标的, 消费者行为]
    quote: "Management is doing things right; leadership is doing the right things."

  - id: wangxiaobo
    name: 王小波
    name_en: Wang Xiaobo
    aliases: [王小波]
    source: panmax/nuwa-skill
    domain: [自由, 理性, 黑色幽默, 批判性思维, 文学]
    trigger_keywords: [自由, 理性, 黑色幽默, 批判, 趣味, 文学创作, 環境与个人]
    avoid: [商业模式, 投资理财, 技术实现]
    quote: "人所具有的一切，不外乎两些：理性的聽命和情感的对象。"

  - id: aurelius
    name: 马可·奥勒留
    name_en: Marcus Aurelius
    aliases: [奥勒留, Marcus Aurelius, 沉思录]
    source: panmax/nuwa-skill
    domain: [斯多葛哲学, 自我修炼, 逆境定力, 决策再平静]
    trigger_keywords: [斯多葛, 自我修炼, 内心宁静, 逆境, 情绪控制, 沉思录, 当下]
    avoid: [商业竞争, 投资, 技术]
    quote: "You have power over your mind, not outside events. Realize this, and you will find strength."
```
