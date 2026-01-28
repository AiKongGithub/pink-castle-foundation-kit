# NotebookLM Integration Guide

> **Version:** 1.0
> **Last Updated:** 2026-01-28
> **Project:** Content 15,300 - Pink Castle Foundation Kit
> **Tool:** Google NotebookLM (notebooklm.google.com)

---

## Overview

คู่มือนี้อธิบายวิธีใช้ Google NotebookLM เพื่อแปลงเนื้อหา SWP3 (340 ไฟล์) เป็น 9 รูปแบบ content สำหรับโครงการ Content 15,300 ชิ้น

### What is NotebookLM?

NotebookLM คือ AI tool จาก Google ที่สามารถ:
- อ่านและวิเคราะห์เอกสารหลายรูปแบบ
- สร้าง Audio Overview (Podcast-style)
- ตอบคำถามจากเนื้อหา
- สรุปเนื้อหาในรูปแบบต่างๆ

### Supported Source Types

| Source Type | Status | Notes |
|-------------|--------|-------|
| PDF | ✅ | Recommended |
| Google Docs | ✅ | Direct import |
| Google Slides | ✅ | Direct import |
| Website URLs | ✅ | Public pages only |
| YouTube Videos | ✅ | Transcription available |
| Text Files | ✅ | .txt, .md |
| Audio/Video Files | ⚠️ | Via YouTube or transcript |

---

## Content Production Workflow

```
┌────────────────────────────────────────────────────────────────┐
│                 NOTEBOOKLM WORKFLOW                            │
├────────────────────────────────────────────────────────────────┤
│                                                                 │
│   ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌─────────┐ │
│   │ PREPARE  │───►│  UPLOAD  │───►│ GENERATE │───►│ EXPORT  │ │
│   │ Sources  │    │    to    │    │ Content  │    │ & Save  │ │
│   │          │    │NotebookLM│    │          │    │         │ │
│   └──────────┘    └──────────┘    └──────────┘    └─────────┘ │
│        │               │               │               │       │
│        ▼               ▼               ▼               ▼       │
│   - Transcripts   - Create new    - Use prompts   - Download   │
│   - PDFs          - Add sources   - Generate      - Copy text  │
│   - Organize      - Verify load   - Review        - Archive    │
│                                                                 │
└────────────────────────────────────────────────────────────────┘
```

---

## Step-by-Step: Audio Overview

Audio Overview เป็น feature หลักของ NotebookLM - สร้าง podcast 2 คนคุยกันจากเนื้อหา

### Step 1: Prepare Source Content

1. **รวบรวม Transcript/เนื้อหา**
   - ถ้าเป็นวิดีโอ: ดึง transcript จาก YouTube หรือ transcribe ด้วย Whisper
   - ถ้าเป็นเอกสาร: แปลงเป็น PDF หรือ Google Doc

2. **จัดรูปแบบเนื้อหา**
   ```
   # [ชื่อบท/หัวข้อ]

   ## Key Points
   - Point 1
   - Point 2

   ## Main Content
   [เนื้อหาหลัก]

   ## Summary
   [สรุป]
   ```

3. **ตรวจสอบคุณภาพ**
   - ไม่มี typos มากเกินไป
   - เนื้อหาสมบูรณ์
   - ความยาวเหมาะสม (ไม่เกิน 50 pages หรือ 500,000 words)

### Step 2: Create Notebook

1. ไปที่ [notebooklm.google.com](https://notebooklm.google.com)
2. คลิก **"New Notebook"**
3. ตั้งชื่อ: `SWP3 - [Chapter Name] - [File Name]`
   - Example: `SWP3 - Ch9 - ไอเดียค้นหาธุรกิจที่ใช่`

### Step 3: Add Sources

1. คลิก **"Add source"**
2. เลือกประเภท:
   - **Google Drive**: สำหรับ Docs/Slides
   - **Upload**: สำหรับ PDF
   - **Website**: สำหรับ URL
   - **YouTube**: สำหรับวิดีโอ
3. รอให้ NotebookLM process (1-5 นาที)
4. ตรวจสอบว่า source ถูกเพิ่มสำเร็จ

### Step 4: Generate Audio Overview

1. คลิกที่ **"Notebook guide"** (มุมขวาบน)
2. คลิก **"Audio Overview"**
3. รอ generate (5-15 นาที ขึ้นอยู่กับความยาว)
4. ฟังตรวจสอบคุณภาพ

### Step 5: Customize Audio (Optional)

ก่อน generate สามารถ customize ได้:

1. คลิก **"Customize"** ใต้ Audio Overview
2. ใส่ instructions:
   ```
   Focus on:
   - Practical applications
   - Step-by-step processes
   - Key takeaways for Thai entrepreneurs

   Avoid:
   - Too technical jargon
   - Lengthy introductions

   Tone: Friendly, educational, conversational
   Duration: Around 10-15 minutes
   ```

### Step 6: Export & Save

1. **Download Audio**
   - คลิก Download icon
   - บันทึกเป็น: `SWP3-Ch[XX]-[FileName]-audio.wav`

2. **Archive Notebook**
   - เก็บ notebook ไว้สำหรับ reference
   - ตั้งชื่อ folder: `NotebookLM-SWP3-Archives`

---

## Prompts for Each Format

### 1. Audio Overview Customization

```
Create an engaging podcast-style audio about this content.

Instructions:
- Target audience: Thai entrepreneurs and business owners
- Duration: 10-15 minutes
- Language: Mix Thai keywords with English terms where appropriate
- Focus on practical, actionable advice
- Include real-world examples
- End with clear takeaways

Tone: Professional but friendly, like two experts having a coffee chat
```

### 2. Video Summary Script

```
Create a video script from this content:

Structure:
1. Hook (5 seconds) - Attention grabber
2. Intro (30 seconds) - What they'll learn
3. Main Points (5-7 minutes) - Key concepts with examples
4. Summary (1 minute) - Quick recap
5. CTA (15 seconds) - What to do next

Format:
- [VISUAL]: Description of what to show
- [NARRATION]: What to say
- [TEXT ON SCREEN]: Key text overlays

Language: Thai with English terms
Target: 8-10 minute video
```

### 3. Mind Map Generation

```
Create a hierarchical mind map from this content.

Requirements:
- Central node: Main topic
- 4-6 main branches: Key themes
- 2-4 sub-branches per main branch
- Use concise text (2-5 words per node)
- Include Thai and English terms

Output format: Mermaid mindmap syntax
Example:
mindmap
  root((Main Topic))
    Branch 1
      Sub 1.1
      Sub 1.2
    Branch 2
      Sub 2.1
```

### 4. Written Report

```
Write a comprehensive report based on this content.

Structure:
1. Executive Summary (100 words)
2. Key Takeaways (5 bullet points)
3. Main Analysis (500-700 words)
   - Context and background
   - Core concepts explained
   - Practical applications
4. Action Items (3-5 items)
5. Source Reference

Language: Thai
Word count: 800-1000 words
Tone: Professional, educational
```

### 5. Flashcards

```
Create flashcards for memorizing key concepts.

Requirements:
- 15-20 Q&A pairs
- Mix of types:
  * Definition (40%): "X คืออะไร?"
  * Concept (30%): "ทำไม X ถึงสำคัญ?"
  * Application (20%): "จะนำ X ไปใช้อย่างไร?"
  * List (10%): "5 องค์ประกอบของ X คืออะไร?"
- Answers: Concise (1-3 sentences)
- Language: Thai

Format:
Q: [Question]
A: [Answer]
```

### 6. Quiz Questions

```
Create a quiz to test understanding of this content.

Requirements:
- 10 questions total
- Mix:
  * 6 Multiple Choice (a, b, c, d)
  * 3 True/False
  * 1 Fill in the blank
- Difficulty: 3 Easy, 4 Medium, 3 Hard
- Each question must have:
  * Clear question text
  * Correct answer
  * Explanation (why correct/incorrect)

Language: Thai
Format:
Q[#]. (Type - Difficulty) Question?
a) Option
b) Option
c) Option
d) Option
Correct: [Letter]
Explanation: [Why]
```

### 7. Infographic Content

```
Extract content for an infographic.

Requirements:
- Title: Catchy, 5-8 words
- 5-7 key points
- Each point: Icon suggestion + Short text (max 10 words)
- Statistics/numbers if available
- Color suggestions based on topic
- Call to action

Format:
TITLE: [Title]

SECTION 1:
Icon: [Suggestion]
Title: [2-3 words]
Text: [Max 10 words]

[Continue for all sections]

CTA: [Action text]
```

### 8. Presentation Slides

```
Create presentation slides from this content.

Requirements:
- 12-15 slides
- Structure:
  1. Title slide
  2. Agenda (4-5 items)
  3-10. Content slides (1 idea per slide)
  11. Summary
  12. Q&A
  13. Call to Action
  14. Thank you

Per slide:
- Title (5-8 words)
- 3-5 bullet points (max 8 words each)
- Visual suggestion
- Speaker notes (2-3 sentences)

Language: Thai
Presentation time: 15-20 minutes
```

### 9. Data Table Extraction

```
Extract structured data from this content into tables.

Table types needed:
1. Key Terms Reference Table
   | Term | Definition | Example |

2. Process/Steps Table
   | Step | Action | Output |

3. Comparison Table (if applicable)
   | Feature | Option A | Option B |

4. Checklist Table
   | Item | Required | Notes |

Requirements:
- Clear headers
- Consistent formatting
- Thai language
- Export-ready (Markdown format)
```

---

## Best Practices for SWP3 Content

### Content Preparation

1. **Video Transcripts**
   - Use Whisper AI or YouTube auto-captions
   - Clean up obvious errors
   - Add speaker labels if multiple speakers
   - Break into paragraphs by topic

2. **Batch Processing**
   - Create notebooks by chapter
   - Add related files to same notebook
   - Use consistent naming convention

3. **Quality Sources**
   - Prefer clean, well-formatted documents
   - Remove duplicate content
   - Include relevant context

### Naming Convention

```
Notebook: SWP3-Ch[XX]-[ShortName]
Audio: SWP3-Ch[XX]-[FileName]-audio-[YYYYMMDD].wav
Report: SWP3-Ch[XX]-[FileName]-report-[YYYYMMDD].md
```

### File Organization

```
Google Drive/
└── NotebookLM-SWP3/
    ├── Sources/
    │   ├── Ch01-ปฐมนิเทศ/
    │   ├── Ch02-8ขั้นตอน/
    │   └── ...
    ├── Outputs/
    │   ├── Audio/
    │   ├── Reports/
    │   ├── MindMaps/
    │   └── ...
    └── Archives/
        └── Notebooks/
```

---

## Limitations & Workarounds

### Known Limitations

| Limitation | Workaround |
|------------|------------|
| Max 50 sources per notebook | Split into multiple notebooks |
| Audio only in English voices | Accept English audio, add Thai subtitles |
| No direct Thai TTS | Use external TTS for Thai audio |
| Processing time varies | Batch process, do other tasks while waiting |
| No API access | Manual process, document for n8n integration |

### Quality Issues

| Issue | Solution |
|-------|----------|
| Audio mispronounces Thai words | Note in content, plan for manual editing |
| Summary misses key points | Provide clearer structure in source |
| Too short/long output | Adjust source length or prompts |
| Hallucinations | Always verify against source |

---

## Time Estimates

### Per Source File

| Activity | Time | Notes |
|----------|------|-------|
| Prepare source | 5-15 min | Depends on format |
| Upload & process | 1-5 min | Automatic |
| Generate audio | 5-15 min | Automatic |
| Generate text content | 2-5 min | Per format |
| Review & export | 5-10 min | Quality check |
| **Total per file** | **20-50 min** | **All 9 formats** |

### Batch Estimates

| Batch Size | Total Time | Efficiency |
|------------|------------|------------|
| 10 files | 4-8 hours | Good for pilot |
| 50 files | 1-2 days | Standard batch |
| 100 files | 3-4 days | With breaks |
| 340 files (all) | 2-3 weeks | Full production |

---

## Integration with Other Tools

### Google Drive
- Source storage
- Output archive
- Sharing for review

### Notion
- Track production status
- QC workflow
- Final content library

### n8n (Future)
- Status update triggers
- File organization automation
- Notification workflows

### Canva
- Infographic design
- Slide beautification
- Thumbnail creation

### Anki/Quizlet
- Flashcard import
- Quiz deployment

---

## Troubleshooting

### Common Issues

**Problem: Source won't upload**
- Check file size (max 500K words)
- Ensure proper format (PDF, Doc)
- Try re-uploading

**Problem: Audio generation stuck**
- Refresh page
- Try different browser
- Check Google account storage

**Problem: Poor audio quality**
- Improve source structure
- Add more context
- Use customization prompts

**Problem: Missing content in summary**
- Break content into smaller sections
- Add explicit headers
- Use bullet points

---

## Quick Reference Card

```
┌─────────────────────────────────────────────┐
│         NOTEBOOKLM QUICK REFERENCE          │
├─────────────────────────────────────────────┤
│                                             │
│ URL: notebooklm.google.com                  │
│                                             │
│ STEPS:                                      │
│ 1. New Notebook                             │
│ 2. Add Source                               │
│ 3. Generate Audio/Content                   │
│ 4. Export & Save                            │
│                                             │
│ NAMING:                                     │
│ SWP3-Ch[XX]-[Name]-[format]-[date]          │
│                                             │
│ TIME:                                       │
│ ~30 min per source (all formats)            │
│                                             │
│ QC:                                         │
│ Always verify against original source       │
│                                             │
└─────────────────────────────────────────────┘
```

---

## Tags

`#notebooklm` `#workflow` `#content-production` `#audio` `#swp3`

---

> *Pink Castle Foundation Kit v1.0*
> *NotebookLM Integration Guide - Content 15,300 Project*
