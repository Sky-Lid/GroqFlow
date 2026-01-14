# GroqFlow 🚀

**The free, blazing-fast, open-source alternative to Wispr Flow**  
Zero-cost voice dictation powered by Groq API + custom AI noise suppression. Speak naturally → clean, polished text appears anywhere. Lightweight Dear ImGui UI (no Electron bloat — low RAM/CPU, instant startup).

Turn your voice into text 3× faster than typing — **forever free**, privacy-focused, and runs on your own Groq API key (free tier available).

### 🌟 Why GroqFlow?
- **Zero subscription cost** — Use your free Groq API key (no limits for light use)
- **Blazing speed** — Groq's ultra-fast inference (sub-second latency on good connections)
- **Superior noise handling** — Built-in improved RNNoise-style denoiser (ReNoiseEF) crushes background noise, echoes, fans — perfect for real-world use (home/office/cafe)
- **Lightweight & snappy** — Dear ImGui + custom backend (no heavy Electron/Chromium) → tiny install, low resource usage, battery-friendly
- **Cross-platform** — Desktop (Windows, macOS, Linux) + mobile support (Android/iOS in progress)
- **Privacy first** — Audio processed via your own Groq key or local fallback (future); no data sent to third parties without consent
- **Fully open-source** — MIT license, hack away!

Wispr Flow charges $15/mo for "unlimited" — GroqFlow gives you unlimited potential for **$0** (beyond your own API usage, which is basically free for personal dictation).

### 🔥 Key Features
- Global hotkey activation (speak anywhere — docs, code, chats, emails)
- Smart AI cleanup & formatting (grammar, punctuation, capitalization via Groq LLM)
- Live VAD (voice activity detection) + real-time denoising
- Customizable prompts/styles (e.g., code mode, casual chat, professional writing)
- Noise-robust: Works great in noisy environments thanks to advanced gain suppression & residuals
- Minimal UI: Status popup, waveform/VAD visualizer, settings — all buttery smooth

### 🚀 Quick Start
1. Get your free Groq API key → [console.groq.com/keys](https://console.groq.com/keys)
2. Clone the repo:
   ```bash
   git clone https://github.com/YOUR_USERNAME/GroqFlow.git
   cd GroqFlow
   ```
3. Install dependencies (Python + PyTorch + Dear ImGui backend — see docs/setup.md)
4. Configure your Groq key in `config.json`
5. Run:
   ```bash
   python main.py  # or build the executable
   ```
6. Press your hotkey (default: Ctrl+Shift+V) → start speaking!

Full setup guide → [docs/setup.md](docs/setup.md)

### 📸 Screenshots / Demo
(Add your screenshots here — e.g., live dictation in VS Code, noisy room demo with/without denoiser)

[Demo video coming soon – record yourself dictating code in a loud room!]

### 🛠️ Tech Stack
- **Backend**: Python, PyTorch, torchaudio, custom ReNoiseEF denoiser (improved RNNoise with residuals, LayerNorm, better gain)
- **Inference**: Groq API (Llama-3 or Mixtral for text polishing)
- **UI**: Dear ImGui (immediate-mode, ultra-lightweight) + GLFW/OpenGL backend
- **Cross-platform**: Works on Windows/macOS/Linux; mobile via Android NDK/Metal (WIP)
- **Features**: STFT/ISTFT pipeline, RMS normalization, VAD gating

### 📖 Documentation
- [Setup & Installation](docs/setup.md)
- [Hotkeys & Customization](docs/hotkeys.md)
- [Denoiser Deep Dive](docs/denoiser.md) — Why it beats basic Whisper noise handling
- [Building Releases](docs/building.md) — Cross-signed binaries, AAB for Android
- [Contributing](CONTRIBUTING.md)

### ⚖️ Comparison vs Wispr Flow
| Feature                  | GroqFlow                  | Wispr Flow              |
|--------------------------|---------------------------|--------------------------|
| Cost                     | $0 (your free Groq key)  | $15/mo Pro              |
| Open Source              | Yes (MIT)                | No                      |
| UI Resource Usage        | Very low (ImGui)         | High (Electron)         |
| Noise Suppression        | Advanced custom model    | Basic                   |
| Latency                  | Sub-second (Groq)        | Fast                    |
| Platforms                | Desktop + Mobile (WIP)   | Desktop + iOS           |
| Privacy                  | Your API key / local opt | Cloud-dependent         |

### 🙌 Contribute
Issues, PRs, ideas welcome! Especially:
- Better mobile support
- More LLM prompt styles
- Local fallback models

Star ⭐ the repo if this saves you money/time — let's build the best free dictation tool together!

Made with ❤️ by an 18-year-old indie dev in Ranchi, India.

#voice-dictation #groq #opensource #wisprflow-alternative #denoising












What do you think — tweak the name, add features, or change tone? Drop your screenshots when ready! 🔥
