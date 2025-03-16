# Ice Breaker - AI驱动的社交破冰助手

Ice Breaker 是一个智能社交助手应用，它能够通过分析LinkedIn和Twitter的公开信息，帮助你更好地了解他人并建立有意义的社交连接。

## 功能特点

- 🔍 自动查找并分析目标人物的LinkedIn和Twitter个人资料
- 📊 生成人物概要和重要事实
- 🎯 识别对方的兴趣爱好
- 💡 提供个性化的破冰话题建议
- 🖼️ 展示个人头像（如果可用）

## 技术栈

- Python 3.x
- Flask (Web框架)
- LangChain (AI链式处理)
- LinkedIn API
- Twitter API

## 安装说明

1. 克隆项目仓库：
```bash
git clone <repository-url>
cd ice_breaker
```

2. 安装依赖：
```bash
# 使用pipenv
pipenv install

```

3. 配置环境变量：
   - 复制`.env.example`文件并重命名为`.env`
   - 填入必要的API密钥和配置信息

## 使用方法

1. 启动应用：
```bash
python app.py
```

2. 在浏览器中访问：`http://localhost:5000`

3. 输入想要了解的人名，系统将自动：
   - 查找其LinkedIn和Twitter账号
   - 分析个人信息
   - 生成会话建议

## 项目结构

```
ice_breaker/
├── agents/          # AI代理模块
├── chains/          # LangChain处理链
├── templates/       # Flask HTML模板
├── static/         # 静态资源文件
├── third_parties/  # 第三方API集成
├── tools/          # 工具函数
├── app.py          # Flask应用入口
├── ice_breaker.py  # 核心业务逻辑
└── output_parsers.py # 输出解析器
```

## 环境要求

- Python 3.8+
- 有效的LinkedIn API密钥
- 有效的Twitter API密钥
- 其他依赖详见`Pipfile`

## 注意事项

- 请确保遵守LinkedIn和Twitter的API使用条款
- 建议在生产环境中添加适当的速率限制
- 注意保护用户隐私和数据安全

## 许可证

本项目采用MIT许可证 - 详见 [LICENSE](LICENSE) 文件
