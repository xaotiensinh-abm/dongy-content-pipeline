# 🏥 Đông Y Content Pipeline — AI Skill

> **Hệ thống sản xuất content Đông Y đa nền tảng**, đóng vai **Bác Sĩ Gia Đình** chuyên cung cấp kiến thức chăm sóc sức khỏe bằng Đông Y tại nhà.

[![Antigravity Skill](https://img.shields.io/badge/Antigravity-Skill-blue)](https://github.com/xaotiensinh-abm)
[![Vietnamese](https://img.shields.io/badge/Language-Vietnamese-red)](.)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## ✨ Tính Năng

- 📚 **Knowledge Base** — 5 files kiến thức Đông Y chuyên sâu (Âm Dương, Ngũ Hành, Kinh Lạc, Thảo dược, 20 bệnh phổ biến)
- 🎭 **Persona & Brand Guide** — Giọng văn Bác Sĩ Gia Đình: thân mật, đồng cảm, dễ hiểu
- 📝 **8 Content Pillars** — Templates chuẩn hóa cho 8 dạng bài viết
- 🧠 **Memory System** — Tracking content + Second Brain cho continuous improvement
- 📅 **12-Week Calendar** — Lộ trình 80+ bài viết chi tiết
- 🔄 **7-Step Pipeline** — Brief → Research → Draft → Style → Quality Gate → Publish → Measure
- 🤖 **Anti-AI Checklist** — 15 tiêu chí đảm bảo nội dung tự nhiên, không AI
- 🌐 **Multi-Platform** — Facebook, Zalo OA, Threads, TikTok, YouTube Shorts

---

## 📁 Cấu Trúc

```
dongy-content-pipeline/
├── SKILL.md                          ← Skill definition (YAML + Instructions)
├── README.md                         ← Hướng dẫn sử dụng
└── resources/
    ├── knowledge-base/               ← Kho kiến thức Đông Y
    │   ├── 01-am-duong.md
    │   ├── 02-ngu-hanh.md
    │   ├── 03-kinh-lac-huyet-vi.md
    │   ├── 04-thao-duoc-gia-dinh.md
    │   └── 05-top20-benh-dieu-tri.md
    ├── persona/
    │   └── brand-guide.md
    ├── templates/
    │   └── content-templates.md
    ├── pipeline/
    │   ├── content-pipeline.md
    │   └── anti-ai-checklist.md
    ├── memory/
    │   ├── content-memory.yaml
    │   └── second-brain.yaml
    ├── calendar/
    │   └── 12-week-calendar.md
    └── examples/
        └── week01/
            └── DY-001-dong-y-gia-dinh.md
```

---

## 🚀 Cách Sử Dụng

### Cài Đặt

Copy thư mục `dongy-content-pipeline/` vào thư mục skills của Antigravity:

```bash
# Windows
copy /r dongy-content-pipeline %USERPROFILE%\.gemini\antigravity\skills\

# macOS/Linux
cp -r dongy-content-pipeline ~/.gemini/antigravity/skills/
```

### Kích Hoạt

Skill tự động kích hoạt khi bạn nói:

```
"viết bài đông y"
"content đông y"
"bác sĩ gia đình"
"chăm sóc sức khỏe đông y"
"thuốc nam"
"huyệt vị"
"thảo dược"
```

### Ví Dụ Sử Dụng

**1. Viết bài mới:**
```
Viết bài DY-003 về mất ngủ, pillar P1, cho Facebook
```

**2. Lên lịch content tuần:**
```
Lên lịch content tuần 3 cho pipeline đông y
```

**3. Viết bài huyệt vị:**
```
Viết bài huyệt Hợp Cốc cho đau đầu, platform Zalo OA
```

---

## 🔄 Pipeline — Quy Trình 7 Bước

```
┌──────────────────────────────────────────────────────────┐
│  1. BRIEF → 2. RESEARCH → 3. DRAFT → 4. STYLE           │
│                                           ↓               │
│  7. MEASURE ← 6. PUBLISH ← 5. QUALITY GATE              │
│                                  ↑         │              │
│                                  └─ FAIL ──┘              │
└──────────────────────────────────────────────────────────┘
```

### Quality Gate

| Gate | Tiêu chuẩn | Ngưỡng PASS |
|------|-----------|-------------|
| Anti-AI Score | Dấu hiệu AI / 15 | ≤ 20% |
| Natural Score | Điểm tự nhiên | ≥ 80/100 |
| Fact-check | Đúng kiến thức Đông Y | OK |
| Compliance | Có disclaimer y tế | OK |

---

## 🎭 Persona — Bác Sĩ Gia Đình

| Yếu tố | Quy tắc |
|---------|---------|
| **Xưng hô** | "Mình" thay vì "tôi", "bạn" thay vì "quý vị" |
| **Giọng văn** | Như người thân khuyên nhủ |
| **Emotional Arc** | Hook → Đồng cảm → Giải thích → Hướng dẫn → Hy vọng |
| **Content Flow** | Thói quen → Biểu hiện → Khắc phục |
| **Tỷ lệ** | Khuyến khích ≥70%, Cảnh báo ≤30% |

---

## 📊 8 Content Pillars

| # | Pillar | Emoji | Ví dụ |
|---|--------|-------|-------|
| P1 | Thói quen → Bệnh | 🔄 | Ngồi lâu → đau lưng |
| P2 | Huyệt vị tự bấm | 📍 | 5 huyệt giảm đau đầu |
| P3 | Thảo dược gia đình | 🌿 | Gừng chữa cảm lạnh |
| P4 | Âm Dương / Ngũ Hành | ☯️ | Tại sao nên ăn theo mùa |
| P5 | Mùa & Dưỡng sinh | 🌸 | Dưỡng sinh mùa hè |
| P6 | Câu chuyện bệnh nhân | 💬 | Chị Lan hết mất ngủ |
| P7 | Myth-busting | ❌ | "Đông Y chậm" — thật không? |
| P8 | Combo: liều trình 7 ngày | 📋 | 7 ngày giảm đau vai gáy |

---

## 🤝 Tích Hợp Với Skills Khác

| Nhu cầu | Skill đề xuất |
|---------|---------------|
| Ảnh minh họa | `nano-banana-pro-master`, `web-image-generator` |
| Video script | `faceless-content-machine`, `veo3-storyboard-director` |
| Audit chất lượng sâu | `content-forge` |
| Xuất PDF | `md-to-pdf` |
| Lập lịch đăng bài | `content-pipeline-orchestrator` |

---

## ⚠️ Lưu Ý Quan Trọng

- **KHÔNG kê đơn thuốc** — Skill này CHỈ chia sẻ kiến thức tham khảo
- **BẮT BUỘC disclaimer** — Mọi bài viết PHẢI có cảnh báo y tế cuối bài
- **Anti-AI check** — Mọi bài PHẢI qua Quality Gate trước khi xuất bản
- **Kiến thức cần verify** — Cross-check với Knowledge Base, không bịa thông tin

---

## 📜 License

MIT License — Sử dụng tự do cho mục đích cá nhân và thương mại.

---

*Được tạo bởi [Antigravity](https://github.com/xaotiensinh-abm) × BMAD-METHOD*
