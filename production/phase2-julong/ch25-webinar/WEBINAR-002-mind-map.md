# Email Marketing Calendar + เทคนิค Powerpoint — WEBINAR-002 Mind Map
> Format: Mind Map / แผนผังความคิด
> Source: SWP3 Ch25 Webinar Mastery ตอนที่ 2
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 3:38:10

---

## Part 1: Text-Based Mind Map

```
                    ┌─────────────────────────────────────────┐
                    │  WEBINAR-002: Email Marketing Calendar   │
                    │  + เทคนิค Powerpoint                     │
                    └────────────────┬────────────────────────┘
                                     │
                ┌────────────────────┼────────────────────┐
                │                    │                    │
     ┌──────────┴──────────┐  ┌─────┴──────┐  ┌─────────┴──────────┐
     │ Email Marketing     │  │ Powerpoint │  │ การบูรณาการ         │
     │ Calendar            │  │ Techniques │  │ Email + Slide       │
     └──────────┬──────────┘  └─────┬──────┘  └─────────┬──────────┘
                │                   │                    │
     ┌──────────┼──────────┐       ┌┼─────────┐        ┌┴───────────┐
     │          │          │       ││         │        │            │
  ┌──┴──┐  ┌───┴──┐  ┌───┴──┐  ┌─┴┴──┐  ┌──┴──┐  ┌──┴──┐  ┌────┴───┐
  │3 เฟส│  │6 ประเภท│  │Auto │  │3 หลัก│  │5 ส่วน│  │CTA  │  │Checklist│
  │     │  │เมล   │  │mation│  │การ   │  │โครง │  │ตรง  │  │ตรวจสอบ  │
  │Pre  │  │      │  │      │  │ออกแบบ│  │สร้าง │  │กัน  │  │ก่อน    │
  │During│  │Invite│  │Trigger│  │      │  │      │  │     │  │Launch  │
  │Post │  │Remind│  │Cond. │  │1 Idea│  │Hook  │  │     │  │        │
  │     │  │Value │  │Logic │  │Visual│  │Problem│ │     │  │        │
  │     │  │Scarce│  │      │  │Story │  │Solution│ │    │  │        │
  │     │  │Thank │  │      │  │      │  │Proof │  │     │  │        │
  │     │  │Replay│  │      │  │      │  │CTA   │  │     │  │        │
  └─────┘  └──────┘  └──────┘  └──────┘  └──────┘  └─────┘  └────────┘
```

---

## Part 2: Mermaid Mind Map

```mermaid
mindmap
  root((WEBINAR-002<br>Email Calendar<br>+ Powerpoint))
    Email Marketing Calendar
      3 เฟส
        Pre-Webinar 4-6 สัปดาห์
        During วันงาน
        Post-Webinar หลังงาน
      6 ประเภทเมล
        Invitation
        Reminder
        Value
        Scarcity
        Thank You
        Replay
      Calendar Structure
        วันที่ส่ง
        เวลาส่ง
        หัวข้อ
        ประเภท
        กลุ่มเป้าหมาย
        CTA
      Segmentation
        ลงทะเบียนแล้ว
        ยังไม่ลงทะเบียน
        เข้าร่วมแล้ว
      Automation
        Trigger Events
        Conditional Logic
        Follow-up Sequence
    Powerpoint Techniques
      หลัก 3 ประการ
        One Idea Per Slide
        Visual First
        Story-Driven
      กฎการออกแบบ
        Font ไม่เกิน 2 แบบ
        สีไม่เกิน 3 โทน
        หัวข้อ 36pt+
        Contrast สูง
      โครงสร้าง 5 ส่วน
        Opening Hook
        Problem Identification
        Solution Framework
        Social Proof
        Call-to-Action
      Animation
        Appear ใช้ได้
        Fade ใช้ได้
        Spin/Bounce ห้ามใช้
    เทคนิคดึงดูดผู้ชม
      สูตร 60-20-10
      Open Loop
      Pattern Interrupt
      Bonus Bribe
      Social Proof ระหว่างงาน
    การบูรณาการ
      เนื้อหาสอดคล้อง
      CTA ทิศทางเดียวกัน
      Checklist ก่อน Launch
```

---

## Part 3: Flowchart — Email Automation Sequence

```mermaid
flowchart TD
    A[ผู้สนใจเข้ามา] --> B{ลงทะเบียน Webinar?}
    B -->|ใช่| C[ส่ง Confirmation Email ทันที]
    B -->|ยัง| D[ส่ง Invitation Email]

    C --> E[รอ 2 วัน]
    E --> F[ส่ง Value Email ให้ความรู้ฟรี]
    F --> G{เปิดอ่าน + คลิก?}

    G -->|เปิด+คลิก| H[รอจนถึงวันก่อนงาน]
    G -->|เปิดไม่คลิก| I[ส่ง Follow-up + Testimonial]
    G -->|ไม่เปิดเลย| J[ส่งซ้ำ Subject Line ใหม่]

    I --> H
    J --> H

    H --> K[ส่ง Reminder 1 วันก่อน]
    K --> L[ส่ง Reminder 1 ชม. ก่อน]
    L --> M[ส่ง Reminder 15 นาทีก่อน]
    M --> N[วัน Webinar]

    D --> O[รอ 3 วัน]
    O --> P[ส่ง Scarcity Email]
    P --> Q{ลงทะเบียน?}
    Q -->|ใช่| C
    Q -->|ยัง| R[ส่ง Last Chance Email]

    N --> S{เข้าร่วม Webinar?}
    S -->|เข้าร่วม| T[ส่ง Thank You + Offer]
    S -->|ไม่เข้าร่วม| U[ส่ง Replay Email]

    T --> V[ส่ง Follow-up Offer 3 วัน]
    U --> V

    style A fill:#FFB6C1,stroke:#333
    style N fill:#90EE90,stroke:#333
    style T fill:#87CEEB,stroke:#333
    style U fill:#FFD700,stroke:#333
```

---

## Part 4: Flowchart — Powerpoint Design Process

```mermaid
flowchart LR
    A[เริ่มออกแบบ] --> B[เลือก Template]
    B --> C[กำหนดสีและ Font]
    C --> D[วางโครงสร้าง 5 ส่วน]

    D --> E[Opening Hook]
    D --> F[Problem]
    D --> G[Solution]
    D --> H[Social Proof]
    D --> I[CTA]

    E --> J[ใส่เนื้อหา<br>1 Idea/Slide]
    F --> J
    G --> J
    H --> J
    I --> J

    J --> K[เพิ่ม Visual<br>รูป/ไอคอน/กราฟ]
    K --> L[ใส่ Animation<br>Appear/Fade เท่านั้น]
    L --> M[วาง Engagement Points<br>ทุก 10-15 นาที]
    M --> N[ทบทวน + ซ้อม]
    N --> O{ผ่านเกณฑ์?}
    O -->|ใช่| P[พร้อม Webinar]
    O -->|ไม่| Q[แก้ไขปรับปรุง]
    Q --> J

    style A fill:#FFB6C1,stroke:#333
    style P fill:#90EE90,stroke:#333
```

---

## Part 5: Flowchart — Webinar Day Timeline

```mermaid
flowchart TD
    A["0-10 นาที<br>Opening Hook + แนะนำตัว"] --> B["10-20 นาที<br>Pattern Interrupt + ถามคำถาม"]
    B --> C["20-40 นาที<br>เนื้อหาหลัก ส่วน 1"]
    C --> D["30 นาที<br>Open Loop วางไว้"]
    D --> E["40-50 นาที<br>เนื้อหาหลัก ส่วน 2"]
    E --> F["50 นาที<br>Pattern Interrupt: Poll/Demo"]
    F --> G["50-60 นาที<br>สรุป + เฉลย Open Loop"]
    G --> H["60-80 นาที<br>นำเสนอ Offer + Bonus Bribe"]
    H --> I["80-90 นาที<br>Q&A + Social Proof ระหว่างงาน"]

    A -.->|"สูตร 60-20-10"| J["60 นาที = เนื้อหา"]
    H -.->|"สูตร 60-20-10"| K["20 นาที = Offer"]
    I -.->|"สูตร 60-20-10"| L["10 นาที = Q&A"]

    style A fill:#FFB6C1,stroke:#333
    style G fill:#FFD700,stroke:#333
    style H fill:#87CEEB,stroke:#333
    style I fill:#90EE90,stroke:#333
```

---

## Part 6: Comparison Diagram — ก่อน vs หลัง เรียนรู้

```
╔══════════════════════════════════════════════════════════════════════╗
║                    ก่อนเรียน vs หลังเรียน                           ║
╠════════════════════════════╦═════════════════════════════════════════╣
║       ก่อนเรียน (แบบเดิม)   ║       หลังเรียน (แบบมืออาชีพ)          ║
╠════════════════════════════╬═════════════════════════════════════════╣
║                            ║                                         ║
║ ส่งเมลแค่ 1 ฉบับ           ║ วางแผน Calendar 3 เฟส 8-12 ฉบับ         ║
║                            ║                                         ║
║ ส่งเมลเดียวกันให้ทุกคน      ║ Segment ตามพฤติกรรม 3 กลุ่ม             ║
║                            ║                                         ║
║ ส่งเมลเอง ลืมบ่อย          ║ Automation + Conditional Logic           ║
║                            ║                                         ║
║ สไลด์ยัดข้อมูลเต็มหน้า      ║ One Idea Per Slide + Visual First       ║
║                            ║                                         ║
║ ไม่มีโครงสร้าง             ║ โครงสร้าง 5 ส่วน (Hook-CTA)              ║
║                            ║                                         ║
║ ผู้ชมออกก่อนจบ 50%+        ║ Open Loop + Pattern Interrupt            ║
║                            ║                                         ║
║ เมลบอกอย่าง สอนอีกอย่าง    ║ เนื้อหาสอดคล้อง CTA ทิศทางเดียวกัน      ║
║                            ║                                         ║
║ ไม่มีแผนหลังงาน            ║ Post-Webinar Sequence + Replay           ║
║                            ║                                         ║
╠════════════════════════════╬═════════════════════════════════════════╣
║ ผลลัพธ์: Show-up 20-30%   ║ ผลลัพธ์: Show-up 50-70%                 ║
║ Conversion: 1-3%          ║ Conversion: 10-20%                       ║
╚════════════════════════════╩═════════════════════════════════════════╝
```

---

## Part 7: Summary Box

```
╔══════════════════════════════════════════════════════════════╗
║                                                              ║
║   สรุป WEBINAR-002: Email Marketing Calendar                ║
║   + เทคนิค Powerpoint                                       ║
║                                                              ║
║   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━   ║
║                                                              ║
║   EMAIL MARKETING CALENDAR                                   ║
║   ● 3 เฟส: Pre-Webinar / During / Post-Webinar              ║
║   ● 6 คอลัมน์: วันที่, เวลา, หัวข้อ, ประเภท, กลุ่ม, CTA     ║
║   ● 6 ประเภทเมล: Invite, Remind, Value, Scarcity,           ║
║     Thank You, Replay                                        ║
║   ● Segment 3 กลุ่ม: สมัครแล้ว / ยังไม่สมัคร / เข้าร่วมแล้ว   ║
║   ● Automation: Trigger + Conditional Logic                  ║
║                                                              ║
║   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━   ║
║                                                              ║
║   POWERPOINT TECHNIQUES                                      ║
║   ● หลัก 3: One Idea / Visual First / Story-Driven          ║
║   ● กฎ: Font 2 แบบ, สี 3 โทน, หัวข้อ 36pt+, Contrast สูง   ║
║   ● โครงสร้าง 5 ส่วน: Hook > Problem > Solution >           ║
║     Social Proof > CTA                                       ║
║   ● Animation: Appear + Fade เท่านั้น                        ║
║                                                              ║
║   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━   ║
║                                                              ║
║   ENGAGEMENT & TIMING                                        ║
║   ● สูตร 60-20-10: 60 นาทีเนื้อหา / 20 Offer / 10 Q&A      ║
║   ● เทคนิค: Open Loop, Pattern Interrupt, Bonus Bribe       ║
║   ● Engagement Point ทุก 10-15 นาที                         ║
║   ● เนื้อหา Email + Slide ต้องสอดคล้องกัน                    ║
║                                                              ║
║   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━   ║
║                                                              ║
║   KEY TAKEAWAY:                                              ║
║   "วางแผนล่วงหน้า ทุกอย่างสอดคล้อง                          ║
║    ทั้ง Email และ Slide ต้องชี้ไปที่เป้าหมายเดียวกัน"          ║
║                                                              ║
╚══════════════════════════════════════════════════════════════╝
```

---

> ทบทวนต่อ: กลับไปดู **WEBINAR-001** หรือไปบทต่อไป
> Series: SWP3 Ch25 Webinar Mastery
> PinkCastle Academy © 2026
