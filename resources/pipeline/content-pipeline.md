# 🔄 CONTENT PIPELINE — QUY TRÌNH SẢN XUẤT END-TO-END

> Workflow chuẩn cho mỗi bài viết trong hệ thống Đông Y Content Pipeline.
> Tích hợp Viet-Pro v3.3 + Anti-AI + Quality Gate.

---

## Pipeline Overview

```
📋 BRIEF → 📚 RESEARCH → ✍️ DRAFT → 🎨 STYLE → 🔍 QUALITY GATE → 📱 PUBLISH → 📊 MEASURE
```

---

## Step 1: 📋 BRIEF — Xác Định Đề Bài

**Input**: Content Calendar (chọn bài tiếp theo)
**Checklist**:
- [ ] Chọn chủ đề từ `calendar/12-week-calendar.md`
- [ ] Xác định: Pillar nào? (P1-P8)
- [ ] Xác định: Platform chính? (FB/TikTok/YouTube/Zalo/IG/LinkedIn/Threads)
- [ ] Check `memory/content-memory.yaml` — bài này đã covered chưa?
- [ ] Xác định linked topics (bệnh liên quan, huyệt liên quan)

**Output**: Brief 1 dòng — Ví dụ: "DY-006 | P1 | Đau vai gáy — thói quen gây ra | FB + Zalo"

---

## Step 2: 📚 RESEARCH — Tra Cứu Kiến Thức

**Input**: Brief
**Sources (ưu tiên)**:
1. `knowledge-base/` — 5 files kiến thức nền tảng (ĐÃ CÓ)
2. Nguồn uy tín: Vinmec, HelloBacsi, sách Đông Y, WHO
3. Cross-reference: Ít nhất 2 nguồn cho mỗi claim y tế

**Checklist**:
- [ ] Tra `05-top20-benh-dieu-tri.md` — protocol có sẵn?
- [ ] Tra `03-kinh-lac-huyet-vi.md` — huyệt nào liên quan?
- [ ] Tra `04-thao-duoc-gia-dinh.md` — thảo dược nào phù hợp?
- [ ] Ghi chú: fact vs opinion
- [ ] List nguồn tham khảo

**Output**: Research notes + Facts verified

---

## Step 3: ✍️ DRAFT — Viết Nháp

**Input**: Research notes + Template từ `templates/content-templates.md`
**Áp dụng**:
- Chọn template đúng Pillar (P1-P8)
- Tuân thủ Persona từ `persona/brand-guide.md`
- Lộ trình BẮT BUỘC: **Thói quen → Biểu hiện → Khắc phục**
- Emotional Arc: **Thấu hiểu → Phân tích → Giải pháp → Hy vọng**

**Checklist**:
- [ ] Hook mở bài — thấu cảm nỗi đau (dưới 20 từ)
- [ ] Phần nguyên nhân — từ thói quen đời thường
- [ ] Triệu chứng — 3-4 dấu hiệu cụ thể
- [ ] Giải pháp — 2-3 cách, hướng dẫn từng bước
- [ ] Kết bài — tích cực, hy vọng
- [ ] CTA + Disclaimer

**Output**: Bài nháp hoàn chỉnh

---

## Step 4: 🎨 STYLE — Biên Tập Phong Cách (Viet-Pro)

**Editors tham gia**:

### Storytelling Editor
- [ ] Hook In Medias Res — bắt đầu từ nỗi đau thật
- [ ] Arc cảm xúc: Tò mò → Căng thẳng → Giải pháp → Hy vọng
- [ ] Bài >= 800 từ phải có case study/nhân vật
- [ ] Kết bài bằng hành động, KHÔNG tóm tắt

### Rhythm Editor
- [ ] Xen kẽ câu ngắn (5 từ) + trung bình (15 từ) + dài (25 từ)
- [ ] Câu nhịp 1-3 từ sau đoạn dài: "Đúng vậy." / "Nghe quen không?"
- [ ] MXH: 1-2 câu/đoạn
- [ ] Punch line cuối mỗi section

### Natural Editor
- [ ] Đọc to — nghe tự nhiên không?
- [ ] Không lặp cấu trúc "X là Y" liên tiếp
- [ ] Từ nối tự nhiên, không máy móc
- [ ] Xưng hô nhất quán

**Output**: Bài đã chỉnh style

---

## Step 5: 🔍 QUALITY GATE — Kiểm Duyệt

> ⚠️ BÀI PHẢI PASS TẤT CẢ 4 GATE MỚI ĐƯỢC XUẤT BẢN

### Gate 1: Anti-AI Check (<= 20%)
Kiểm tra 15 dấu hiệu AI (xem `anti-ai-checklist.md`):
- [ ] Nhóm A: Từ vựng AI (5 items) → 0 vi phạm
- [ ] Nhóm B: Cấu trúc AI (5 items) → <= 1 vi phạm
- [ ] Nhóm C: Tông giọng AI (5 items) → <= 1 vi phạm
- **Score**: ___/15 vi phạm → ___% (phải <= 20% = <= 3 vi phạm)

### Gate 2: Natural Score (>= 80%)
- [ ] Đọc to toàn bài — nghe như người Việt viết?
- [ ] Không có câu "dịch máy"?
- [ ] Rhythm tự nhiên?
- **Score**: ___/100 (phải >= 80)

### Gate 3: Fact-Check
- [ ] Mọi claim y tế → có nguồn?
- [ ] Công dụng thảo dược → đúng theo Dược điển?
- [ ] Vị trí huyệt → đúng theo giải phẫu?
- [ ] Liều lượng → an toàn?

### Gate 4: Compliance
- [ ] Disclaimer y tế → CÓ
- [ ] Không hứa "chữa khỏi" → OK
- [ ] Không kê đơn / bán thuốc → OK
- [ ] Không nói xấu Tây Y → OK
- [ ] Khuyến khích gặp bác sĩ khi nặng → OK

**Kết quả**: PASS → Step 6 | FAIL → Quay Step 3/4

---

## Step 6: 📱 PUBLISH — Xuất Bản

### 6a. Tối ưu theo platform
- [ ] Facebook: 300-800 từ, emoji vừa phải, ảnh 1200x630
- [ ] TikTok: Script 30-60s, hook 3s, 1 vấn đề = 1 giải pháp
- [ ] Instagram: Carousel 5-7 slides, 1 slide = 1 ý chính
- [ ] Zalo OA: 200-400 từ, thân mật, lời chào mùa
- [ ] YouTube: 5-15 phút, demo huyệt/nấu thuốc
- [ ] LinkedIn: 200-500 từ, wellness angle chuyên nghiệp
- [ ] Threads: 100-200 từ, 1 tip ngắn

### 6b. Repurpose Flow
```
📝 Bài gốc (FB)
 ├→ TikTok script (phần Khắc phục)
 ├→ IG carousel (5-7 slides)
 ├→ Zalo (rút gọn 300 từ)
 ├→ LinkedIn (góc wellness)
 ├→ Threads (1 quote + 1 tip)
 └→ YouTube (mở rộng + demo)
```

### 6c. Lên lịch đăng
- [ ] Khung giờ vàng: 7:00-8:00 (sáng) hoặc 20:00-21:00 (tối)

---

## Step 7: 📊 MEASURE & LEARN — Đo Lường & Học Hỏi

### Cập nhật Memory
- [ ] Thêm entry vào `content-memory.yaml` → published_content
- [ ] Cập nhật topic_coverage
- [ ] Cập nhật herbs_introduced / acupoints_taught
- [ ] Cập nhật pillar_distribution

### Cập nhật Second Brain (cuối tuần)
- [ ] Ghi learning_log: Bài nào tốt? Vì sao?
- [ ] Cập nhật performance_patterns
- [ ] Ghi nhận audience_feedback
- [ ] Cập nhật knowledge_gaps nếu có câu hỏi mới

---

## Checklist Nhanh (In ra dán bàn)

```
☐ Brief → đề bài rõ ràng
☐ Research → kiến thức chính xác
☐ Draft → đúng template + persona  
☐ Style → storytelling + rhythm + natural
☐ Anti-AI <= 20%
☐ Natural >= 80%
☐ Fact-check OK
☐ Disclaimer CÓ
☐ Publish → tối ưu platform
☐ Repurpose → >= 3 platforms
☐ Memory update
```
