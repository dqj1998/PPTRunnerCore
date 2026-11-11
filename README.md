# PPTRunner Core (pptrunner-core)

> **Video as Code for Presentations**  
> AI 原生的声明式 PPT 视频编译引擎：将静态幻灯片转换为高保真、音画精准对齐的交互式视频。

---

### 💡 核心设计理念

传统的 AI 视频工具往往是不可解释、无法敏捷维护的黑盒。`PPTRunner Core` 采用类似于编译器的结构化处理管线：

1. **PPT 解析**：提取幻灯片的二维空间拓扑、视觉权重与上下文意图。
2. **Markdown 脚本**：大模型智能重构口语化讲义台词与重音停顿标记。
3. **YAML分镜头**：声明式定义镜头排期、局部放大/高亮目标及音画微观时间轴。
4. **HTML/JS 动效**：基于现代 Web 标准组件（Remotion / SVG / CSS）驱动局部动态聚焦。
5. **本地极速渲染**：通过 Headless Chrome 与 FFmpeg 在本地无状态容器中产出 MP4/WebM。

### 🔒 隐私与安全性保障 (Local-First & Zero-Data-Leak)

* **本地闭环执行**：PPT 原件、解说脚本、分镜头配置文件及最终视频全程留在本地网络环境。
* **BYOK 架构**：无缝对接企业内部自有的 LLM 与 TTS 端点（如 Azure OpenAI、AWS Bedrock 或本地部署的开源模型）。
* **透明可审计**：纯代码开源，专为企业安全合规审查（情シス/CISO）设计。
