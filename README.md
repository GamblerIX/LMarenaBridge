# 🤖 LMArena-API

> **免费使用 Claude、GPT-4、Gemini 等顶级 AI 模型的桌面工具**

LMArena-API 是一款桌面应用，让你无需付费订阅，就能在各种 AI 客户端中使用 Claude、GPT-4、Gemini 等多种顶级大语言模型，通过逆向技术将LMArena.ai平台的所有模型转为兼容OpenAI格式，实现API调用。

---

## 软件截图

<table style="width:100%; border-collapse:collapse;">
  <tr>
    <td style="text-align:center; padding:6px;">
      <img src="E:\work\promotion\LMArena-api\images\image-20251210172449076.png" width="90%" alt="image-20251210172449076" />
    </td>
    <td style="text-align:center; padding:6px;">
      <img src="E:\work\promotion\LMArena-api\images\image-20251210172527772.png" width="90%" alt="image-20251210172527772" />
    </td>
  </tr>
  <tr>
    <td style="text-align:center; padding:6px;">
      <img src="E:\work\promotion\LMArena-api\images\image-20251210172607869.png" width="90%" alt="image-20251210172607869" />
    </td>
    <td style="text-align:center; padding:6px;">
      <img src="E:\work\promotion\LMArena-api\images\image-20251210172708851.png" width="90%" alt="image-20251210172708851" />
    </td>
  </tr>
</table>

## 🎯 这款工具适合谁？

| 👤 用户类型 | 使用场景 | 推荐客户端 |
|------------|---------|-----------|
| **日常用户** | 与 AI 对话、写作辅助、问答 | Cherry Studio |
| **程序员** | AI 辅助编程、代码审查、Debug | Roo Code (VS Code 插件) |
| **翻译用户** | 网页翻译、文档翻译、字幕翻译 | 沉浸式翻译 |
| **开发者** | 在自己的程序中调用 AI 接口 | 直接调用 API |

---

## 🚀 30 秒快速开始

### 第一步：下载安装

从 [GitHub Releases](https://github.com/jtostrings/LMarenaBridge/releases) 下载对应版本：

| 操作系统 | 下载文件 | 说明 |
|---------|---------|------|
| **Windows** | `LMArena-API.7z` | 解压即用，无需安装 |
| **macOS-inter芯片** | `LMArena-API-mac-x64` | 拖入应用程序文件夹 |
| **macOS-M芯片** | LMArena-API-mac-arm64 | 拖入应用程序文件夹 |

### 第二步：启动并配置（约 2 分钟）

1. **启动应用** → 运行 LMArena-API
2. **创建客户端** → 进入「浏览器客户端」页面 → 点击「新建客户端」
3. **网站条款验证** → 在弹出的页面中发送任意一条消息
4. **启动服务** → 回到「服务控制」页面 → 点击「启动服务」

✅ 完成！现在你的本地 API 服务已在 `http://127.0.0.1:61001` 运行

### 第三步：配置你的 AI 客户端

在任意支持 OpenAI API 的客户端中填写：

| 配置项 | 值 |
|-------|-----|
| **API 地址** | `http://127.0.0.1:61001` 或 `http://127.0.0.1:61001/v1` |
| **API 密钥** | `123456`（可在应用「配置管理」中修改） |
| **模型** | 从应用「模型管理」中选择任意模型 |

---

## 📱 主流客户端配置教程

### Cherry Studio（AI 对话客户端）

Cherry Studio 是一款跨平台的 AI 对话客户端，界面美观，功能丰富。

**配置步骤：**

1. 打开 Cherry Studio → 设置 → 添加新的 API 提供商
2. 选择「OpenAI Compatible」（OpenAI 兼容）
3. 填写配置信息：
   - **API 地址：** `http://127.0.0.1:61001`
   - **API 密钥：** `123456`

4. 保存并测试连接

![Cherry Studio 测试](https://cdn.nlark.com/yuque/0/2025/png/21449790/1764234560775-dc916a1c-3832-4f6f-9e2d-db51f13b3bf5.png)

---

### Roo Code（VS Code AI 编程助手）

Roo Code 是一个强大的 VS Code AI 编程插件，类似于 Cursor AI。

**配置步骤：**

1. 在 VS Code 扩展市场安装 **Roo Code**
2. 打开插件设置 → 选择「Custom/自定义提供商」
3. 填写配置：
   - **Base URL：** `http://127.0.0.1:61001/v1`
   - **API Key：** `123456`
   - **Model：** 选择你想用的模型

![Roo Code 配置](https://cdn.nlark.com/yuque/0/2025/png/21449790/1763097509817-2d94ce58-b798-42d3-b3da-abbe025a0ee4.png)

**现在你可以：**
- 💬 与 AI 对话讨论代码问题
- ✍️ 让 AI 帮你编写代码
- 🔍 让 AI 审查和优化代码
- 🐛 协助调试和修复 Bug

---

### 沉浸式翻译（网页/文档翻译）

[沉浸式翻译](https://immersivetranslate.com/) 是一款优秀的网页翻译扩展，配合顶级 AI 模型，翻译质量远超传统翻译。

**配置步骤：**

1. 安装沉浸式翻译浏览器扩展
2. 打开扩展设置 → 翻译服务 → 选择「OpenAI」
3. 切换到「自定义 API」
4. 填写配置：
   - **API URL：** `http://127.0.0.1:61001/v1/chat/completions`
   - **API Key：** `123456`
   - **模型：** 选择你想用的 AI 模型

![沉浸式翻译配置](https://cdn.nlark.com/yuque/0/2025/png/21449790/1764234788903-b0759b29-176d-4930-a2e1-3d138a32da1c.png)

**现在你可以：**
- 🌐 用顶级 AI 模型翻译网页
- 📄 翻译 PDF 文档
- 📺 翻译视频字幕

---

## 💻 开发者 API 调用指南

如果你是开发者，想在自己的程序中调用 API，请参考以下示例。

### API 端点

| 端点 | 方法 | 说明 |
|-----|------|------|
| `/v1/chat/completions` | POST | OpenAI 兼容的聊天接口 |
| `/v1/models` | GET | 获取可用模型列表 |

### Python 代码示例

#### 流式响应（实时输出）

适合需要实时显示 AI 回复的场景：

<details>
<summary><b>📋 点击展开代码</b></summary>

```python
import requests
import json

# API 配置
url = "http://127.0.0.1:61001/v1/chat/completions"
API_KEY = "123456"

headers = {
    "Content-Type": "application/json",
    "Authorization": f"Bearer {API_KEY}"
}

payload = {
    "model": "claude-sonnet-4-20250514",
    "messages": [
        {"role": "user", "content": "你好，请介绍一下你自己"}
    ],
    "stream": True
}

def stream_chat():
    response = requests.post(url, headers=headers, json=payload, stream=True, timeout=180)
    response.raise_for_status()
    
    for line in response.iter_lines():
        if line:
            line_str = line.decode('utf-8')
            if line_str.startswith('data:'):
                json_str = line_str[len('data: '):].strip()
                if json_str == '[DONE]':
                    break
                try:
                    data = json.loads(json_str)
                    content = data.get('choices', [{}])[0].get('delta', {}).get('content', '')
                    if content:
                        print(content, end='', flush=True)
                except json.JSONDecodeError:
                    continue

if __name__ == "__main__":
    stream_chat()
```

</details>

#### 非流式响应（等待完整回复）

适合不需要实时显示的场景：

<details>
<summary><b>📋 点击展开代码</b></summary>

```python
import requests

# API 配置
url = "http://127.0.0.1:61001/v1/chat/completions"
API_KEY = "123456"

headers = {
    "Content-Type": "application/json",
    "Authorization": f"Bearer {API_KEY}"
}

payload = {
    "model": "claude-sonnet-4-20250514",
    "messages": [
        {"role": "user", "content": "你好，请介绍一下你自己"}
    ]
}

def chat():
    response = requests.post(url, headers=headers, json=payload, timeout=180)
    response.raise_for_status()
    
    data = response.json()
    content = data['choices'][0]['message']['content']
    print(f"AI 回复：{content}")
    return data

if __name__ == "__main__":
    chat()
```

</details>

---

## ⚙️ 应用功能说明

### 服务控制

- 一键启动/停止 API 服务
- 实时显示服务运行状态和时长

### 浏览器客户端管理

- **新建客户端：** 创建独立的浏览器会话
- **预览/隐藏：** 实时查看客户端页面状态
- **多客户端支持：** 创建多个客户端可提高并发处理能力

### 配置管理

- API 密钥设置（默认 `123456`）
- 端口配置（默认 `61001`）
- 内容长度限制
- 备用模型池设置

### 模型管理

- 查看所有可用 AI 模型
- 按名称、提供商搜索过滤
- 一键更新模型列表

---

## ❓ 常见问题

<details>
<summary><b>授权码如何获取？</b></summary>
请通过以下方式联系作者，

微信: tostring1 (如果扫码失败, 请直接搜索微信号)
备用 QQ: 854569279

<img src="https://camo.githubusercontent.com/6aea6c36266495b86e5b9cc4e5071ac10f6160f66dfe5c86aecf70a0ae2b56a3/68747470733a2f2f63646e2e6e6c61726b2e636f6d2f79757175652f302f323032352f706e672f32313434393739302f313736343634323636353133342d39333564633736302d323363632d343136342d623538352d3434356263343431616439642e706e67" width="200" />

</details>

### 安装与启动

<details>
<summary><b>macOS 提示「无法打开」或「已损坏」？</b></summary>

这是 macOS 的安全保护机制。解决方法：

**方法一（推荐）：**
1. 点击「取消」关闭提示
2. 打开「系统设置」→「隐私与安全性」
3. 滚动到底部，点击「仍要打开」

**方法二：** 右键点击应用 → 选择「打开」

</details>

<details>
<summary><b>端口 61001 被占用？</b></summary>

- 应用会自动尝试终止占用端口的进程
- 或在「配置管理」中修改端口号

</details>

### 使用问题

<details>
<summary><b>模型列表为空？</b></summary>

1. 确保至少创建了一个浏览器客户端
2. 点击「模型管理」中的「更新模型列表」按钮

</details>

<details>
<summary><b>API 请求没有响应？</b></summary>

1. 检查服务是否正在运行
2. 查看应用底部日志面板的错误信息
3. 确认模型名称是否正确

</details>

<details>
<summary><b>如何提高并发处理能力？</b></summary>

在「浏览器客户端」页面创建更多客户端，每个客户端都是独立的会话，可以并行处理请求。

</details>

<details>
<summary><b>遇到 429 错误如何解决？</b></summary>

请在「浏览器客户端」页面删除当前客户端，新建一个客户端并完成验证（发送任意消息），即可恢复使用。

</details>



---

## ✨ 特性一览

- ✅ 跨平台支持（Windows / macOS）
- ✅ 绿色版，解压即用，无需安装
- ✅ 兼容 OpenAI API 格式
- ✅ 内置浏览器客户端，无需外部依赖
- ✅ 支持多客户端负载均衡
- ✅ 现代化暗色主题界面
- ✅ 实时日志查看

---

## 📜 许可证

MIT License

## 🙏 致谢

- [LMArena](https://lmarena.ai) - AI 模型评估平台
- [Electron](https://www.electronjs.org/)
- [React](https://react.dev/)
