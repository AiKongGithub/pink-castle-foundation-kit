# Data Table Template

> **Format:** Data Table (ตารางข้อมูล)
> **Tool:** NotebookLM + Google Sheets/Notion
> **Output:** Structured data extract
> **Type:** Reference table, comparison, or database

---

## Purpose

Extract and organize key information from source content into structured tables that can be used for reference, comparison, or data analysis.

---

## Template Structure

### Table Types

#### 1. Reference Table
```
| Term | Definition | Example | Category |
|------|------------|---------|----------|
| [Term 1] | [Definition] | [Example] | [Cat] |
| [Term 2] | [Definition] | [Example] | [Cat] |
```

#### 2. Comparison Table
```
| Feature | Option A | Option B | Option C |
|---------|----------|----------|----------|
| [Feature 1] | [Value] | [Value] | [Value] |
| [Feature 2] | [Value] | [Value] | [Value] |
```

#### 3. Process Table
```
| Step | Action | Tools | Output | Time |
|------|--------|-------|--------|------|
| 1 | [Action] | [Tools] | [Output] | [Time] |
| 2 | [Action] | [Tools] | [Output] | [Time] |
```

#### 4. Checklist Table
```
| Item | Required | Status | Notes |
|------|----------|--------|-------|
| [Item 1] | Yes/No | [ ] | [Notes] |
| [Item 2] | Yes/No | [ ] | [Notes] |
```

#### 5. Statistics Table
```
| Metric | Value | Benchmark | Status |
|--------|-------|-----------|--------|
| [Metric 1] | [Value] | [Target] | [Status] |
| [Metric 2] | [Value] | [Target] | [Status] |
```

---

## NotebookLM Prompt

```
Extract structured data from this content and create tables that:
1. Organize key information logically
2. Use appropriate table types
3. Include all important data points
4. Have clear headers
5. Can be exported to spreadsheet
6. Are in Thai where appropriate
7. Include source reference
```

---

## Example Output

**Source:** บทที่ 10: Youtube Marketing Mastery

### Table 1: Youtube Metrics Reference

| Metric | Thai Name | Definition | Good Benchmark |
|--------|-----------|------------|----------------|
| CTR | Click-Through Rate | % คนที่คลิกดู | 5-10% |
| Watch Time | เวลาดู | นาทีที่คนดูรวม | มากที่สุดเท่าที่จะได้ |
| AVD | Average View Duration | เวลาดูเฉลี่ย | >50% of video |
| Retention | การคงอยู่ | % ที่ดูถึงจุดต่างๆ | >40% at end |
| Subscribers | ผู้ติดตาม | จำนวนคนติดตามช่อง | เพิ่มต่อเนื่อง |
| Engagement | การมีส่วนร่วม | Likes + Comments | >5% of views |
| Impressions | การแสดงผล | จำนวนครั้งที่โชว์ | ยิ่งมากยิ่งดี |

---

### Table 2: Content Type Comparison

| Content Type | Effort | Engagement | Watch Time | Best For |
|--------------|--------|------------|------------|----------|
| Tutorial | High | High | High | Building authority |
| Vlog | Medium | Medium | Medium | Personal connection |
| Shorts | Low | High | Low | Discovery |
| Interview | Medium | Medium | High | Credibility |
| List/Ranking | Low | High | Medium | Viral potential |
| Review | Medium | Medium | Medium | Trust building |
| Live Stream | Low | High | High | Community |

---

### Table 3: Video Optimization Checklist

| Element | Action | Importance | Status |
|---------|--------|------------|--------|
| Title | Include keyword at start | Critical | [ ] |
| Thumbnail | High contrast, face, text | Critical | [ ] |
| Description | First 100 chars keyword-rich | High | [ ] |
| Tags | 5-10 relevant tags | Medium | [ ] |
| Chapters | Add timestamps | Medium | [ ] |
| End Screen | Link to other videos | High | [ ] |
| Cards | Add 2-3 cards | Medium | [ ] |
| Subtitles | Add Thai captions | Medium | [ ] |
| Pinned Comment | Add CTA | Low | [ ] |
| Playlist | Add to relevant playlist | Medium | [ ] |

---

### Table 4: Youtube Tools Comparison

| Tool | Purpose | Price | Best For |
|------|---------|-------|----------|
| TubeBuddy | SEO & Keywords | Free-$49/mo | Keyword research |
| VidIQ | Analytics & SEO | Free-$49/mo | Competitor analysis |
| Canva | Thumbnails | Free-$13/mo | Design |
| Zubtitle | Captions | Free-$19/mo | Subtitles |
| OBS | Recording | Free | Live streaming |
| Camtasia | Editing | $250 one-time | Screen recording |
| DaVinci | Editing | Free-$295 | Professional editing |

---

### Table 5: Upload Schedule by Channel Size

| Subscribers | Recommended Frequency | Min. Quality | Focus |
|-------------|----------------------|--------------|-------|
| 0-1K | 1-2/week | Good | Consistency |
| 1K-10K | 2-3/week | Good | Niche focus |
| 10K-100K | 3-4/week | Great | Growth |
| 100K+ | 4-7/week | Excellent | Scale |

---

## Data Format Guidelines

### Markdown Format
```markdown
| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Data 1 | Data 2 | Data 3 |
```

### CSV Format
```csv
Header 1,Header 2,Header 3
Data 1,Data 2,Data 3
```

### JSON Format
```json
[
  {"field1": "value1", "field2": "value2"},
  {"field1": "value3", "field2": "value4"}
]
```

---

## Quality Checklist

### Content Quality
- [ ] All key data points included
- [ ] Information is accurate
- [ ] Data is current
- [ ] Sources are cited

### Structure
- [ ] Headers are clear
- [ ] Data is categorized
- [ ] Consistent formatting
- [ ] Logical order

### Usability
- [ ] Easy to scan
- [ ] Searchable
- [ ] Exportable
- [ ] Updatable

### Technical
- [ ] Works in spreadsheets
- [ ] Proper data types
- [ ] No merge issues
- [ ] Clean data

---

## QC Scoring (ปลัดซัน)

| Criteria | Weight | Score (1-5) | Notes |
|----------|--------|-------------|-------|
| Data Accuracy | 30% | | |
| Completeness | 25% | | |
| Structure | 25% | | |
| Usability | 20% | | |
| **Total** | 100% | | |

**Pass Threshold:** 70% (3.5/5 average)

---

## Export Formats

- Markdown (.md)
- CSV (.csv)
- Google Sheets
- Notion database
- Excel (.xlsx)
- JSON

---

## Use Cases

| Use Case | Table Type | Example |
|----------|------------|---------|
| Terminology | Reference | Glossary of terms |
| Decision Making | Comparison | Tool comparison |
| Implementation | Process | Step-by-step guide |
| Audit | Checklist | Optimization checklist |
| Reporting | Statistics | KPI dashboard |

---

## Tags

`#datatable` `#reference` `#notebooklm` `#spreadsheet` `#structured`

---

> *Pink Castle Foundation Kit v1.0*
