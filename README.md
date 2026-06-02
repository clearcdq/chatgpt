# ChatGPT 资源集合

![License](https://img.shields.io/badge/License-MIT-blue.svg) ![Awesome](https://awesome.re/badge.svg) ![Status](https://img.shields.io/badge/Status-Active-success)

> 🚀 ChatGPT 使用指南、代理工具、免费节点获取方式和相关资源的集合

## 📋 项目概述

本仓库汇集了 **ChatGPT 使用技巧**、**网络代理工具**、**免费节点获取方式** 以及其他相关资源，帮助用户更好地访问和使用 ChatGPT 服务。

## ✨ 主要内容

### 1. 🧭 ChatGPT 使用指南
- ChatGPT 官方注册和使用教程
- 常见问题解决方案
- 提示词（Prompt）编写技巧
- API 调用示例和最佳实践

### 2. 🔀 代理工具（梯子）
- VPN 推荐
- 代理软件列表
  - Clash
  - Shadowsocks
  - Trojan
  - V2Ray
- 配置教程和最佳实践

### 3. 🌍 免费节点获取
- 免费代理节点资源
- 节点订阅链接
- 节点质量评估方法
- 定期更新的节点列表

### 4. 🛠️ 相关工具和脚本
- ChatGPT 自动化脚本
- 批量获取 API Key 的方法
- 会话管理工具
- 成本优化方案

## 🚀 快速开始

### 基础使用

```bash
# 克隆仓库
git clone https://github.com/clearcdq/chatgpt.git
cd chatgpt

# 查看文档
ls docs/

# 查看代理配置
ls proxy-configs/
```

### 推荐工作流

1. **第一步**：阅读 `docs/getting-started.md` 了解基础
2. **第二步**：选择合适的代理工具（参考 `proxy-tools/recommendations.md`）
3. **第三步**：获取免费节点或付费订阅
4. **第四步**：配置代理并访问 ChatGPT

## 📂 目录结构

```
chatgpt/
├── README.md                          # 本文件
├── docs/                              # 文档目录
│   ├── getting-started.md            # 快速开始
│   ├── faqs.md                       # 常见问题
│   ├── prompts.md                    # 提示词库
│   └── api-guide.md                  # API 使用指南
├── proxy-tools/                       # 代理工具
│   ├── clash/                        # Clash 配置
│   ├── shadowsocks/                  # SS 配置
│   ├── v2ray/                        # V2Ray 配置
│   ├── trojan/                       # Trojan 配置
│   └── recommendations.md            # 工具对比
├── nodes/                             # 免费节点资源
│   ├── free-nodes.txt               # 免费节点列表
│   ├── node-checker.py              # 节点检测脚本
│   └── subscription-links.md         # 订阅链接
├── scripts/                           # 自动化脚本
│   ├── get-api-key.py               # 获取 API Key
│   ├── bulk-test.py                 # 批量测试
│   └── auto-proxy.sh                # 自动代理配置
└── resources/                         # 其他资源
    ├── reference-links.md            # 参考链接
    └── paid-services.md              # 付费服务推荐
```

## 🔧 工具对比

| 工具 | 平台 | 易用性 | 性能 | 功能 | 推荐度 |
|------|------|--------|------|------|--------|
| Clash | Win/Mac/Linux | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | 强大 | ⭐⭐⭐⭐⭐ |
| Shadowsocks | 全平台 | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ | 简单 | ⭐⭐⭐⭐ |
| V2Ray | 全平台 | ⭐⭐⭐ | ⭐⭐⭐⭐ | 很强 | ⭐⭐⭐⭐ |
| Trojan | 全平台 | ⭐⭐⭐ | ⭐⭐⭐⭐ | 中等 | ⭐⭐⭐ |

## 📚 使用提示

### 获取免费节点

```bash
# 方式1：从仓库获取
cat nodes/free-nodes.txt

# 方式2：使用检测脚本验证节点
python3 scripts/node-checker.py

# 方式3：订阅链接（长期更新）
# 参考 nodes/subscription-links.md
```

### 配置 Clash

1. 下载 Clash 客户端
2. 导入配置文件或订阅链接
3. 选择节点并启用系统代理
4. 访问 ChatGPT

### 使用 API Key

```python
import openai

# 设置 API Key
openai.api_key = "your-api-key-here"

# 调用 API
response = openai.ChatCompletion.create(
    model="gpt-3.5-turbo",
    messages=[
        {"role": "user", "content": "Hello!"}
    ]
)
```

## 💡 最佳实践

### 安全建议

1. **不要分享 API Key** - 将其妥善保管
2. **使用专用账户** - 创建仅用于代理的账户
3. **定期更换节点** - 避免单点故障
4. **监控流量** - 定期检查使用情况
5. **法规合规** - 遵守当地法律法规

### 性能优化

- 选择距离近的节点
- 避免高峰时段使用
- 使用 HTTP/3 (QUIC) 协议
- 启用连接复用

## ⚠️ 免责声明

- 本仓库仅供学习和研究使用
- 不保证节点的稳定性和可用性
- 免费节点可能存在安全风险，使用时需谨慎
- 用户应自行承担使用本仓库内容的风险
- 遵守 OpenAI 的使用条款和当地法律法规

## 🤝 贡献指南

欢迎贡献！

### 如何贡献

1. Fork 本仓库
2. 创建功能分支 (`git checkout -b feature/xxx`)
3. 提交更改 (`git commit -m 'Add xxx'`)
4. 推送分支 (`git push origin feature/xxx`)
5. 开启 Pull Request

### 贡献内容

- 新节点资源
- 改进的配置文件
- 有用的脚本
- 文档改进

## 📞 联系方式

- **GitHub Issues** - 提问和反馈
- **Discussions** - 讨论话题
- **Email** - clearcdq@gmail.com

## 📄 许可证

本项目采用 **MIT 许可证**，详见 [LICENSE](LICENSE)

## 🙏 致谢

感谢所有贡献者和社区支持！

---

**最后更新**: 2026年6月  
**维护者**: [@clearcdq](https://github.com/clearcdq)  
**⭐ 如果有帮助，请给个 Star！**
