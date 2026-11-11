# PPTRunner Core (pptrunner-core)

> **Video as Code for Presentations**  

---

### 💡 Core Design Philosophy

Traditional AI video tools often function as "black boxes"—opaque, uninterpretable, and difficult to maintain or adapt. `PPTRunner Core` utilizes a structured, compiler-like processing pipeline:

1. **PPT Parsing**: Extracts the 2D spatial topology of slides, visual weighting, and contextual intent.
2. **Markdown Scripting**: Leverages Large Language Models (LLMs) to intelligently reconstruct spoken-word scripts, complete with emphasis and pause markers.
3. **YAML Storyboarding**: Declaratively defines shot sequencing, targeted zooms/highlights, and precise audio-visual timelines.
4. **HTML/JS Animation**: Drives dynamic, localized focus using modern web standards (Remotion, SVG, and CSS).
5. **High-Speed ​​Local Rendering**: Generates MP4/WebM files within a local, stateless container using Headless Chrome and FFmpeg.

### 🔒 Privacy and Security (Local-First & Zero-Data-Leak)

* **Local Closed-Loop Execution**: All source PPT files, scripts, storyboard configurations, and final videos remain entirely within your local network environment.
* **BYOK (Bring Your Own Key/Model) Architecture**: Integrates seamlessly with your organization’s existing LLM and TTS endpoints (e.g., Azure OpenAI, AWS Bedrock, or locally deployed open-source models).
* **Transparent and Auditable**: Fully open-source code, designed specifically to meet enterprise security and compliance standards (IT/CISO review).
