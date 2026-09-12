# BUSINESS ANALYSIS YAŞVARI DÖVRƏSI METODOLOJI
## BA Lifecycle Approach - Daxili Sorğu Sistemi Layihəsi

---

## 📖 Giriş

Bu sənəd, Daxili Sorğu İdarəetmə Sistemi layihəsində istifadə olunan Business Analysis yaşvari dövrəsinin (BA Lifecycle) tamamını ətraflı şəkildə təsvir edir.

**BA Lifecycle**, layihənin **bəşərə başlanğıcından tamamlanması sonuna qədər** Business Analyst-lərin fəaliyyətlərini müəyyən edən strukturlaşdırılmış prosesdir.

---

## 🔄 BA Lifecycle Overview

### Mərhələlər Strukturu

```
┌────────────────────────────────────────────────────────────────┐
│                                                                │
│   1. INITIATION          → Problemin müəyyənləşdirilməsi      │
│        ↓                                                        │
│   2. PLANNING & ANALYSIS → Tələblərin toplanması & Analizi    │
│        ↓                                                        │
│   3. SOLUTION DESIGN     → Həllin tasarlanması                │
│        ↓                                                        │
│   4. IMPLEMENTATION      → Developerlərlə əməkdaşlıq          │
│        ↓                                                        │
│   5. TESTING & VALIDATION → Keyfiyyətin yoxlanması            │
│        ↓                                                        │
│   6. EVALUATION          → Nəticələrin ölçülməsi              │
│        ↓                                                        │
│   📊 CONTINUOUS MONITORING & OPTIMIZATION                      │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```

---

## 🎬 MƏRHƏLƏ 1: BAŞLANĞIÇ (INITIATION)

### Məqsəd
Layihənin əsasını qoymaq, problemin dərinə anlaşılmasını təmin etmək və stakeholderlərin razılığını əldə etmək.

### Əsas Fəaliyyətlər

#### **1.1 Problem Dönarı Müəyyənləşdirmə**

**Sual:** Hansı problemin həlli üçün bu layihə qurulacaq?

```
PROBLEM STATEMENT

Hazırda Vəziyyət:
└─ Daxili xidmət sorğuları email və qeyri-formal əlaqə ilə idarə olunur
   ├─ Manual emal prosesləri
   ├─ Standartlaşdırılmış iş axınlarının olmaması
   └─ Şəffaf izləmə mexanizminin olmaması

Nəticədə:
└─ Sorğular 5-7 işçi günə gedər (Target: 2-3 gün)
└─ İstifadəçilər sorğu statusunu bilmir (Target: 100% görünürlük)
└─ SLA-ları izləmə mümkün olmur (Target: 90% compliance)
└─ Reklama xərclərər artır (Target: 40% azalma)
```

#### **1.2 Stakeholder Tanımlaması & Analizi**

**Sual:** Bu layihədən kim fəaldir?

```
STAKEHOLDER MAP

Yüksək Əhəmiyyətli & Yüksək Gücü:
├─ CEO / Direktor (Sponsor)
├─ HR Departament Başçısı (Product Owner)
└─ İT Müdürü (Technical Lead)

Yüksək Əhəmiyyətli & Düşük Gücü:
├─ İstifadəçilər (Employees)
├─ Audit & Compliance
└─ Finance (Büdcə kontrol)

Düşük Əhəmiyyətli & Yüksək Gücü:
├─ Vendor / System Integrator
└─ External Consultants

Düşük Əhəmiyyətli & Düşük Gücü:
└─ İçəri haberci (Internal newsletter)
```

**Stakeholder Analiz Matrisi:**

| Stakeholder | Rolü | Əhəmiyyət | Güc | Strategiya |
|-------------|------|----------|-----|-----------|
| CEO | Sponsor | Çox Yüksək | Çox Yüksək | Manage Closely |
| HR Başçı | Product Owner | Çox Yüksək | Yüksək | Manage Closely |
| İT Müdürü | Technical Lead | Yüksək | Yüksək | Manage Closely |
| Employees | End Users | Yüksək | Orta | Keep Satisfied |
| Audit | Regulator | Orta | Orta | Keep Informed |
| Finance | Budget Owner | Orta | Yüksək | Keep Satisfied |

#### **1.3 Fərziyyələrin (Assumptions) Dönarı Müəyyənləşdirmə**

```
ASSUMPTIONS LOG

Assumption 1: Stakeholders layihəyə 100% dəstək verir
└─ Dəyişmə ihtimalı: Aşağı
└─ Təsiri: Yüksək (kritik)
└─ Məqsəd: Düzenli iclaslar keçmək

Assumption 2: Budget 200,000 AZN həddinə keçməyəcək
└─ Dəyişmə ihtimalı: Orta
└─ Təsiri: Yüksək
└─ Məqsəd: Scope kontrol, value vs. cost

Assumption 3: Xarici sistem inteqrasiyasına ehtiyac olmayacaq (Year 1)
└─ Dəyişmə ihtimalı: Orta
└─ Təsiri: Orta
└─ Məqsəd: Architecture flexibility qurulması

Assumption 4: Mövcud 200+ əməkçi sistem istifadə etməlidir
└─ Dəyişmə ihtimalı: Aşağı
└─ Təsiri: Yüksək
└─ Məqsəd: Training & change management
```

#### **1.4 Risklərin Müəyyənləşdirilməsi**

```
RISK LOG

Risk 1: Stakeholder əlaqasının kəsilməsi
├─ Ehtimal: Orta (50%)
├─ Təsir: Yüksək (project deadline-i pozabilir)
├─ Azaltma: Monthly steering committee meetings
└─ Sorumlu: Project Manager

Risk 2: Tələblərin dəyişmə
├─ Ehtimal: Yüksək (70%)
├─ Təsir: Orta (schedule delay)
├─ Azaltma: Change control board, frozen requirements
└─ Sorumlu: Product Owner

Risk 3: User adoption başarısızlığı
├─ Ehtimal: Orta (40%)
├─ Təsir: Yüksək (project faildır)
├─ Azaltma: Comprehensive training, early engagement
└─ Sorumlu: Change Manager

Risk 4: Technical complexity
├─ Ehtimal: Orta (45%)
├─ Təsir: Orta (schedule delay)
├─ Azaltma: Prototype, POC, experienced team
└─ Sorumlu: Technical Lead
```

#### **1.5 SMART Məqsədləri Qurulması**

```
LAYIHƏ MƏQSƏDLƏRI (SMART)

S - SPECIFIC (Spesifik):
"Daxili sorğuların mərkəzləşdirilmiş platformada idarə olması"

M - MEASURABLE (Ölçülən):
┌──────────────────────────────────────┐
│ KPI                                  │
├──────────────────────────────────────┤
│ Emal müddəti: 5-7 gün → 3-4 gün    │
│ İzlənə bilənlik: 40% → 100%        │
│ SLA uyğunluğu: 60% → 90%           │
│ Manual işlərin azalması: 50%        │
│ Sistem uptime: 99%+                 │
└──────────────────────────────────────┘

A - ACHIEVABLE (Həyata Keçərilə Bilən):
✓ Mövcud texnologiya yetərlidir
✓ Budget uygun
✓ Təcrübəli team mövcuddur

R - RELEVANT (Uyğun):
✓ Strategik ehtiyacları ödəyir
✓ Stakeholder istəklərinə uyğundur

T - TIME-BOUND (Vaxtı Müəyyən):
Tətbiq: 6 ay (26 həftə)
MVP: 3 ay
Go-live: 6 ay
```

#### **1.6 Scope Qurulması**

```
SCOPE STATEMENT

IN SCOPE (Daxil):
✅ Sorğuların yaradılması & izlənməsi
✅ Avtomatik iş axınları
✅ SLA idarəetməsi
✅ Performans hasabatları
✅ Notification sistemi
✅ Audit logging

OUT OF SCOPE (Xaricində):
❌ Xarici sistem inteqrasiyaları
❌ Mobil tətbiq (ilk mərhələdə)
❌ HR payroll inteqrasiyası
❌ Müştəri xidməti portalı

DEPENDENCIES (Bağlılıqlar):
→ IT infrastructure hazır olmalı
→ Active Directory inteqrasiyası
→ Database şəbəkə qurulması
```

#### **1.7 Tamamlanmış Sənədlər**

✅ **Problem Statement & Business Need** (1-2 səhifə)
✅ **Stakeholder Analysis & Map** (RACI Matrix)
✅ **Assumptions & Risk Log** (Excel Sheet)
✅ **High-Level Success Criteria** (SMART Goals)
✅ **Project Charter** (Rəsmən təsdiqli)

### Çıktılar (Deliverables)
- ✅ Approved Charter
- ✅ Stakeholder Register
- ✅ High-Level Scope Statement

---

## 📊 MƏRHƏLƏ 2: PLANLAŞDIRMA & ANALIZ (PLANNING & ANALYSIS)

### Məqsəd
Cari vəziyyəti (AS-IS) və gələcək vəziyyəti (TO-BE) ətraflı anlamaq, boşluqları tanımlamaq, tələbləri ətraflı şəkildə toplamaq.

### Əsas Fəaliyyətlər

#### **2.1 Tələblərin Toplanması (Elicitation)**

**Tələb Toplamaq Üsulları:**

```
ELICITATION TECHNIQUES

1️⃣ INTERVIEWS (Müsahibə)
   └─ One-on-one stakeholder meetings
   └─ Semi-structured questions
   └─ Duration: 30-45 min
   └─ Participants: 10+ stakeholders

2️⃣ WORKSHOPS (İş Sessiyaları)
   └─ Group brainstorming sessions
   └─ Collaborative requirements mapping
   └─ Duration: 2-3 saat
   └─ Participants: 15-20 people

3️⃣ DOCUMENT REVIEW (Sənəd İnceləməsi)
   └─ Current process documentation
   └─ Previous system specs
   └─ Email conversations
   └─ Existing forms & templates

4️⃣ OBSERVATION (Müşahidə)
   └─ Current workflow observation
   └─ Job shadowing
   └─ Process walkthrough
   └─ Duration: 8-10 saat

5️⃣ SURVEYS (Sorğu)
   └─ Online questionnaires
   └─ Likert scale questions
   └─ Open-ended feedback
   └─ Participants: 50+ employees
```

**Elicitation Plan:**

| Tarix | Teknik | Katılımcılar | Odak Noktası |
|-------|--------|-------------|--------------|
| W1 | Interviews | HR Başçı, Managers | Business needs |
| W2 | Workshops | Power users, HR | Current process |
| W2-3 | Observation | End users | Workflow details |
| W3 | Interviews | IT Team | Technical constraints |
| W4 | Surveys | All employees | User expectations |

#### **2.2 Cari Durum (AS-IS) Analizi**

```
CURRENT STATE ANALYSIS

SORĞU YARATıLMASI PROSESI (AS-IS):

1. Müştəri Email Gönderir
   ↓
2. HR Mailbox-u Kontrol Edir
   ├─ Vəzifə: Excel spreadsheet-ə yazır
   └─ Vaxt: 30-60 dəqiqə
   ↓
3. Manager Məsul Şəxsi Tapır
   └─ Vaxt: 24-48 saat
   ↓
4. İmam Qərəzin Təfərrüatını Toplayır
   ├─ Əsasən Phone Call
   └─ Vaxt: 24-48 saat
   ↓
5. İcra (Manual iş)
   └─ Vaxt: 1-3 gün
   ↓
6. Müştəriyə Qaytar
   ├─ Email ilə
   └─ Vaxt: 24 saat
   ↓
7. Total Müddət: 5-7 işçi günü ⚠️

PROBLEMLər:
❌ Email spam folderinə düşə biləri
❌ İşçi tərəfindən yadda qaçabilər
❌ Duplicate requests mövcud
❌ Prioritetlər aydınlıq yoxdur
❌ Sorğu statusu görünmür
```

#### **2.3 Gələcək Durum (TO-BE) Analizi**

```
FUTURE STATE ANALYSIS

SORĞU YARATıLMASI PROSESI (TO-BE):

1. Müştəri Web Portal-da Sorğu Yaradır
   ├─ Ayrıntılar avtomatik toplanır
   └─ Vaxt: 5-10 dəqiqə
   ↓
2. Sistem Avtomatik Yönləndirir
   ├─ Business rules əsasında
   └─ Vaxt: <1 dəqiqə (otomatik)
   ↓
3. Məsul Şəxs Bildirişi Alır
   ├─ Email + Platform notification
   └─ Vaxt: Ani
   ↓
4. İcra (Manual iş)
   └─ Vaxt: 1-2 gün
   ↓
5. Müştəriyə Avtomatik Qaytar
   ├─ Status güncelləməsi
   └─ Vaxt: Ani
   ↓
6. Total Müddət: 2-3 işçi günü ✅

FAYDALANANCıLAR:
✅ Sorğu hiçbir zaman itəmir
✅ Avtomatik yönləndirmə (insan xətası yoxdur)
✅ Real-time status tracking
✅ SLA alerts otomatik
✅ Performance data otomatik toplanır
```

#### **2.4 Gap Analysis (Boşluq Analizi)**

```
GAP ANALYSIS TABLE

Fəaliyyət          | AS-IS           | TO-BE           | Gap | Çözüm
─────────────────────────────────────────────────────────────────
Sorğu Yaradılması  | Email           | Web Form        | ✓   | Portal dev
Yönləndirmə        | Manual          | Otomatik        | ✓   | Workflow engine
Prioritetləşdirmə  | Qeyri-formal    | Rules-based     | ✓   | Business rules
İzləmə             | Spreadsheet     | Database        | ✓   | Real-time tracking
SLA Kontrol        | Manual          | Otomatik Alert  | ✓   | SLA engine
Hasabat            | Manual Excel    | Real-time Dash  | ✓   | Analytics module
Audit Trail        | Yoxdur          | Full logging    | ✓   | Audit logs
Notification       | Email only      | Multi-channel   | ✓   | Notification eng.

ROOT CAUSE ANALYSIS (5 WHYS):

Problem: Sorğular 5-7 gün çəkir

Why 1: Yönləndirmə manuel
Why 2: Məsul şəxsi tapmaq çətin
Why 3: Yönləndirmə qaydaları yoxdur
Why 4: Sistem mərkəzləşdirilməyib
→ Root Cause: Mərkəzləşdirilmiş sistem yoxdur

Həll: Mərkəzləşdirilmiş MIS sistemi qurulması
```

#### **2.5 Tələblərin Sənədləşdirilməsi**

```
BUSINESS REQUIREMENTS (BR - İş Tələbləri)

BR-001: Tamamlayıcı müqavimətli sorğu idarəetməsi
────────────────────────────────────────────────────
Açıqlama: Sistem bütün daxili sorğuları vahid platformada idarə etməlidir
Əhəmiyyət: Critical
Müqavimətçi: HR Başçı
Test Kriteri: Tüm sorğular sistemdə yaradıla biləri

BR-002: Sorğuların status real-time görünməsi
────────────────────────────────────────────────────
Açıklama: İşçilər sorğularının her an statusunu görebiləri
Əhəmiyyət: High
Müqavimətçi: End Users
Test Kriteri: Dashboard 5 saniyə azında güncelle edilən

BR-003: SLA-ların otomatik nəzarəti
────────────────────────────────────────────────────
Açıklama: Sistem vəzifə müddətləri izləmiş, gecikmişləri alert etməlidir
Əhəmiyyət: High
Müqavimətçi: Management
Test Kriteri: SLA ihlal 1 saat əvvəl alert verilən

FUNCTIONAL REQUIREMENTS (FR - Funksional Tələblər)

FR-001: Sorğu yaradılması formu
────────────────────────────────
Sistem aşağıdakı sahələrin olduğu bir form göstərməlidir:
├─ Sorğu Tipi (Dropdown: HR, IT, Finance, etc.)
├─ Açıklama (Text Area)
├─ Əhəmiyyət (Radio: Low, Medium, High)
├─ Due Date (Date Picker)
└─ Attachment (File upload)

Priority: High
Acceptance Criteria:
├─ Form javascript validation edən
├─ File size max 10MB
└─ Bütün sahələr required-dır

FR-002: Sorğu durumu dashboard-u
──────────────────────────────────
Sistem bir dashboard göstərməlidir:
├─ New requests: X
├─ In Progress: Y
├─ Completed: Z
└─ Overdue: W

Priority: High
Acceptance Criteria:
├─ Dashboard 5 saniyə əvvəl güncelle edilən
├─ Color coding (Green, Yellow, Red)
└─ Export to Excel imkanı

NON-FUNCTIONAL REQUIREMENTS (NFR - Qeyri-Funksional Tələblər)

NFR-001: PERFORMANCE (Performans)
─────────────────────────────────
├─ Page load time < 2 seconds
├─ Database query response < 500ms
├─ Support 500 concurrent users
└─ 99% uptime requirement

NFR-002: SECURITY (Təhlükəsizlik)
──────────────────────────────────
├─ SSL/TLS encryption
├─ Active Directory integration
├─ Role-based access control
├─ Audit trail logging
└─ Password policy enforcement

NFR-003: USABILITY (İstifadəçi Dostu)
──────────────────────────────────────
├─ Responsive design (mobile-friendly)
├─ Intuitive navigation
├─ Max 3 clicks to complete task
└─ Multi-language support (AZ, RUS, ENG)

NFR-004: MAINTAINABILITY (Təmir Edilə Bilənlik)
────────────────────────────────────────────────
├─ Modular architecture
├─ Code documentation
├─ Regular backups
└─ Disaster recovery plan
```

#### **2.6 Requirements Traceability Matrix (RTM)**

```
REQUIREMENTS TRACEABILITY MATRIX (RTM)

ID    | Tələb              | Test Case | Status  | Notes
------|-------------------|-----------|---------|--------
BR-001| Sorğu idarəetməsi  | TC-001    | Design  | -
BR-002| Real-time status   | TC-002    | Design  | -
BR-003| SLA monitoring     | TC-003    | Design  | -
FR-001| Sorğu formu        | TC-101    | Dev     | Sprint 1
FR-002| Dashboard          | TC-102    | Design  | Sprint 2
FR-003| Workflow engine    | TC-103    | Design  | Sprint 2
NFR-001| Performance       | TC-201    | Design  | -
NFR-002| Security          | TC-202    | Design  | -

Traceability:
├─ Business requirement → Functional requirements
├─ Functional req → Test cases
├─ Test cases → Implementation
└─ Implementation → Documentation
```

#### **2.7 Tamamlanmış Sənədlər**

✅ **Elicitation & Communication Plan**
✅ **Current State (AS-IS) Documentation**
✅ **Future State (TO-BE) Documentation**
✅ **Gap Analysis Report**
✅ **Business Requirements Document (BRD)**
✅ **Requirements Traceability Matrix (RTM)**
✅ **Change Impact Assessment** (varsa)

### Çıktılar
- ✅ Business Requirements List (25+ BR)
- ✅ Stakeholder Communication Plan
- ✅ Approved RTM

---

## 🎨 MƏRHƏLƏ 3: HƏLL DİZAYNI (SOLUTION DESIGN)

### Məqsəd
Tətbiq etməsi üçün sistem spesifikasyonlarını hazırlamaq, diaqramlar çəkmək, user stories yazmaq.

### Əsas Fəaliyyətlər

#### **3.1 Use Case Diagram**

```
USE CASE DIAGRAM

           ┌─────────────────────────────┐
           │   Internal Request System   │
           └─────────────────────────────┘
                        │
        ┌───────┬───────┼───────┬───────┐
        │       │       │       │       │
        ▼       ▼       ▼       ▼       ▼
     ┌────┐ ┌────┐ ┌────┐ ┌────┐ ┌────┐
     │ UC1│ │ UC2│ │ UC3│ │ UC4│ │ UC5│
     └────┘ └────┘ └────┘ └────┘ └────┘
      │      │      │      │      │
      │      │      │      │      │
      ▼      ▼      ▼      ▼      ▼
    Create Track Update Approve Generate
    Request Status Request Request Report

   ACTORS:
   - Employee (Request Creator)
   - Manager (Approver)
   - HR Admin (Request Handler)
   - System (Automated workflows)
```

#### **3.2 Data Flow Diagram (DFD)**

```
DATA FLOW DIAGRAM - LEVEL 0 (CONTEXT DIAGRAM)

┌──────────────┐           External Entities
│  Employees   │◄──────────
└──────────────┘           ┌─────────────────┐
       │                    │  MAIL GATEWAY   │
       │ Requests           └─────────────────┘
       │
       ▼
   [0] MIS System
       │
       │ Status Updates
       │ Notifications
       │
       ▼
┌──────────────┐
│   Dashboard  │
│   & Reports  │
└──────────────┘

DATA FLOW DIAGRAM - LEVEL 1 (DETAILED)

┌──────────┐
│ Employee │
└──────────┘
     │
     │ 1.0: Create Request
     │
     ▼
┌───────────────┐
│ Request Form  │
│ Validation    │
└───────────────┘
     │
     │ Valid Request
     │
     ▼
┌───────────────┐
│ Workflow      │
│ Engine        │
└───────────────┘
     │
     ├─→ 2.0: Assign to Handler
     ├─→ 3.0: Send Notification
     └─→ 4.0: Update Status

┌───────────────┐
│ Database      │ ◄─── Data Storage
│ (Requests,    │
│ Status,       │
│ History)      │
└───────────────┘
     │
     │ Data
     │
     ▼
┌───────────────┐
│ Report Engine │ ◄─── 5.0: Generate Reports
└───────────────┘
     │
     │ Reports/Dashboards
     │
     ▼
[Employee Dashboard & Reports]
```

#### **3.3 Entity Relationship Diagram (ERD)**

```
ENTITY RELATIONSHIP DIAGRAM

┌─────────────────┐
│   EMPLOYEE      │
├─────────────────┤
│ ID (PK)         │
│ Name            │
│ Email           │
│ Department      │
│ Role            │
└──────┬──────────┘
       │
       │ 1:N
       │
       ▼
┌─────────────────┐       ┌──────────────┐
│   REQUEST       │       │  REQUEST     │
├─────────────────┤       │  STATUS      │
│ ID (PK)         │◄──────┤──────────────┤
│ Employee_ID (FK)│   N:1 │ ID (PK)      │
│ Type            │       │ Name         │
│ Description     │       │ Description  │
│ Priority        │       └──────────────┘
│ Created_Date    │
│ Due_Date        │
│ Status_ID (FK)  │
│ Handler_ID (FK) │
│ Updated_Date    │
└──────┬──────────┘
       │
       │ 1:N
       │
       ▼
┌─────────────────┐
│   COMMENT       │
├─────────────────┤
│ ID (PK)         │
│ Request_ID (FK) │
│ Employee_ID (FK)│
│ Comment_Text    │
│ Created_Date    │
└─────────────────┘

┌─────────────────┐
│   ATTACHMENT    │
├─────────────────┤
│ ID (PK)         │
│ Request_ID (FK) │
│ File_Path       │
│ File_Size       │
│ Uploaded_Date   │
└─────────────────┘
```

#### **3.4 BPMN Process Diagram**

```
BPMN PROCESS DIAGRAM

[Start] ──→ ┌─────────────────┐
            │ Create Request  │
            │ (Employee)      │
            └────────┬────────┘
                     │
                     ▼
            ┌─────────────────┐
            │ Validate        │
            │ Request         │
            └────────┬────────┘
                     │
          ┌──────────┴──────────┐
          │                     │
        Invalid             Valid
          │                     │
          ▼                     ▼
     ┌────────────┐      ┌─────────────────┐
     │ Show Error │      │ Route to        │
     │ Message    │      │ Appropriate Dept│
     └────────────┘      └────────┬────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │ Assign to       │
                         │ Responsible    │
                         │ Person         │
                         └────────┬────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │ Send            │
                         │ Notification    │
                         └────────┬────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │ Process Request │
                         │ (Manual Work)   │
                         └────────┬────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │ Complete &      │
                         │ Update Status   │
                         └────────┬────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │ Notify Employee │
                         │ (Completion)    │
                         └────────┬────────┘
                                  │
                                  ▼
                              [End]
```

#### **3.5 User Stories & Acceptance Criteria**

```
USER STORY FORMAT

USER STORY #1: Create Request

As an [EMPLOYEE]
I want to [CREATE AND SUBMIT A SERVICE REQUEST]
So that [I CAN GET THE HELP I NEED]

ACCEPTANCE CRITERIA:
✓ Employee can fill in a form with:
  - Request Type (dropdown)
  - Description (text area)
  - Priority (radio button)
  - Due Date (date picker)
  - Attachment (file upload)

✓ System validates all required fields
✓ System accepts files up to 10MB
✓ Confirmation message shows after submission
✓ Request ID is displayed for tracking
✓ Email confirmation is sent

PRIORITY: High
STORY POINTS: 5
SPRINT: Sprint 1


USER STORY #2: Track Request Status

As an [EMPLOYEE]
I want to [SEE THE CURRENT STATUS OF MY REQUEST]
So that [I KNOW WHEN TO EXPECT A RESOLUTION]

ACCEPTANCE CRITERIA:
✓ Dashboard shows all my requests
✓ Each request shows:
  - Request ID
  - Submission Date
  - Current Status (New/In Progress/Completed)
  - Days Pending
  - Responsible Person

✓ Color coding: Green (On track), Yellow (At risk), Red (Overdue)
✓ Can filter by status, date range, priority
✓ Can search by Request ID
✓ Export to Excel functionality

PRIORITY: High
STORY POINTS: 8
SPRINT: Sprint 2


USER STORY #3: Receive Notifications

As a [REQUEST HANDLER]
I want to [RECEIVE AUTOMATIC NOTIFICATIONS]
So that [I DON'T MISS NEW REQUESTS]

ACCEPTANCE CRITERIA:
✓ Notification sent immediately when assigned
✓ Notification includes:
  - Request ID
  - Description
  - Priority
  - Due Date
  - Requestor Contact

✓ Multiple notification channels:
  - Email
  - SMS (optional)
  - In-app notification

✓ Can snooze notifications
✓ Can configure notification preferences

PRIORITY: High
STORY POINTS: 5
SPRINT: Sprint 2
```

#### **3.6 Business Rules**

```
BUSINESS RULES

BR-1: Request Priority Assignment
Rule: Requests are automatically prioritized based on:
      ├─ Request Type (HR requests = High)
      ├─ Department (Finance = Critical)
      ├─ Keywords in description ("urgent", "asap")
      └─ Business impact level
Implementation: Workflow engine rule engine

BR-2: SLA Time Calculation
Rule: Each request type has a max resolution time:
      ├─ HR Requests: 2 business days
      ├─ IT Requests: 1 business day
      ├─ Finance: 3 business days
      └─ Other: 5 business days
Implementation: Timer and alert system

BR-3: Escalation Rules
Rule: If request exceeds 75% of SLA time:
      ├─ Send reminder to handler
      ├─ Notify manager
      └─ Flag as "At Risk"
Implementation: Workflow engine

BR-4: Auto-Assignment
Rule: New requests are automatically assigned to:
      ├─ Based on request type
      ├─ Load balancing (fewest active requests)
      └─ Skill matching
Implementation: Workflow engine with AI

BR-5: Duplicate Prevention
Rule: System detects and flags potential duplicates:
      ├─ Same requestor + similar description
      ├─ Within last 30 days
      └─ Suggests linking or consolidating
Implementation: Fuzzy matching algorithm

BR-6: Approval Workflow
Rule: Requests requiring approval must:
      ├─ Route to appropriate approver
      ├─ Wait for approval before processing
      ├─ Allow approval/rejection with comments
      └─ Track approval history
Implementation: Approval matrix + workflow
```

#### **3.7 Tamamlanmış Sənədlər**

✅ **Functional Requirements (FR) - 35+**
✅ **Non-Functional Requirements (NFR) - 15+**
✅ **Use Case Diagram**
✅ **Data Flow Diagrams (DFD)**
✅ **Entity Relationship Diagram (ERD)**
✅ **BPMN Process Diagram**
✅ **User Stories (40+)**
✅ **Acceptance Criteria**
✅ **Business Rules (20+)**
✅ **Context Diagram**
✅ **Data Dictionary**

### Çıktılar
- ✅ Complete Solution Design Document
- ✅ Technical Specification
- ✅ Development Roadmap

---

## 🔧 MƏRHƏLƏ 4: TƏTBIQ (IMPLEMENTATION SUPPORT)

### Məqsəd
Desarrollo teamə dəstək olmaq, tələblərin aydınlaşdırılması, change management.

### Əsas Fəaliyyətlər

- 📋 Requirement Clarifications
- 🔄 Change Request Handling
- 📞 Developer Collaboration
- ✅ Quality Assurance Liaison
- 📝 Technical Documentation Support

---

## ✅ MƏRHƏLƏ 5: SÜNAQ & VALIDASIYA (TESTING & VALIDATION)

### Məqsəd
Sistemin gereksinimleri karşıladığından emin olmak.

### Əsas Fəaliyyətlər

- 🧪 UAT Plan
- 📋 Test Cases
- ❌ Error Scenarios
- ✓ Acceptance Criteria

---

## 📊 MƏRHƏLƏ 6: QIYMƏTLƏNDIRMƏ (EVALUATION)

### Məqsəd
Layihənin məqsədləri işəldərdinə çatıb çatmadığını ölçmək.

### Əsas Fəaliyyətlər

- 📈 KPI Measurement
- ✅ Success Metrics
- 📝 Post-Implementation Report
- 🎓 Lessons Learned

---

## 📚 BA TOOLS & TEMPLATES

### Istifadə Olunan Alətlər

| Alət | Məqsəd |
|------|--------|
| Google Docs | Sənəd yazılması |
| Google Sheets | Traceability & tracking |
| Lucidchart | Diaqram çəkilməsi |
| Draw.io | UML diaqramları |
| Miro | Brainstorming sessions |

### Istifadə Olunan Şablonlar

- User Story Template
- Use Case Template
- Test Case Template
- Requirements Traceability Matrix
- Risk Register
- Assumptions Log
- Change Request Log

---

## 📖 Əsas Xülasə

```
BA LIFECYCLE Summary

1. INITIATION
   └─ Problem defined, stakeholders identified, scope set

2. PLANNING & ANALYSIS
   └─ Requirements gathered, AS-IS/TO-BE analyzed, gaps identified

3. SOLUTION DESIGN
   └─ Technical specs created, diagrams drawn, user stories written

4. IMPLEMENTATION
   └─ Development team supported, changes managed

5. TESTING & VALIDATION
   └─ System tested, UAT conducted

6. EVALUATION
   └─ Results measured, success criteria evaluated

🎯 Expected Outcome: Fully functional MIS system that meets all
   requirements and delivers business value
```

---

**Hazırlayan:** Business Analysis Team  
**Tarix:** Sentyabr 2024  
**Versiya:** 1.0  
**Status:** ✅ Approved

---

*Bu sənəd BA yaşvari dövrəsinin tamamına dair bir referans sənədidir.*
