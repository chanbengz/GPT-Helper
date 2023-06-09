# 🤖 GPT-Helper
基于Streamlit搭建的GPT低代码漏洞安全审查助手，支持以下功能：

- 审查低代码应用工作流中可能的安全性问题
- 多聊天窗口
- 历史对话留存
- 模型参数调节
- 对话导出为Markdown文件
- ChatGPT语音交流（推荐电脑端Edge浏览器） 
### 使用方法：
- （不选择本地部署）访问``
- 新建对话窗口
- 选择上下文”低代码平台安全检查“
- 输入工作流
- Ctrl + Enter 可快捷提交工作流
- 得到安全建议

# 部署

本地部署需要科学上网。
1. 建立虚拟环境（建议）

2. 进入项目文件夹
```bash
cd GPT-Helper/
```

3. 安装依赖
```bash
pip install -r requirements.txt
```

4. 设置API Key   

- 在 `.streamlit/secrets.toml`文件中写入`apikey = "Your Openai Key"`

5. 启动应用
```bash
streamlit run app.py
```


# 致谢
感谢以下项目作者

- 本项目基于[shan-mx/ChatGPT_Streamlit](https://github.com/shan-mx/ChatGPT_Streamlit)项目进行的改造。
- 预设的[上下文功能](https://github.com/PierXuY/ChatGPT-Assistant/blob/main/set_context.py)参考自[binary-husky/chatgpt_academic](https://github.com/binary-husky/chatgpt_academic)项目和[f/awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)项目。
- 语音交互功能参考了项目[talk-to-chatgpt](https://github.com/C-Nedelcu/talk-to-chatgpt)和[Voice Control for ChatGPT](https://chrome.google.com/webstore/detail/voice-control-for-chatgpt/eollffkcakegifhacjnlnegohfdlidhn)的实现。
