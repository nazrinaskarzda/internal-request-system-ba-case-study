## Business Analysis Case Study (Tam layihə sənədləşdirilməsi)

## Layihə haqqında

Bu case study daxili xidmət sorğularının idarə olunması üçün **mərkəzləşdirilmiş informasiya sisteminin (MIS)** qurulması prosesini əhatə edən tam Business Analysis layihəsinin sənədləşdirilməsidir.

Layihə Business Analysis-in həyat dövrünün tamamını əks etdirir:

- **Başlanğıc (Initiation)** - Problemin müəyyənləşdirilməsi
- **Planlaşdırma və analiz (Planning & Analysis)** - Tələblərin toplanması
- **Həll dizaynı (Solution Design)** - Texniki spesifikasiyalar
- **Tətbiq (Implementation)** - İnkişaf dəstəyi
- **Sınaq və validasiya (Testing & Validation)** - Keyfiyyətin yoxlanılması
- **Qiymətləndirmə (Evaluation)** - Nəticələrin ölçülməsi

## Biznes problemi

### Cari vəziyyət (AS-IS)

Hazırda daxili xidmət sorğuları **qeyri-strukturlaşdırılmış** şəkildə idarə olunur:

- Sorğular e-poçt və digər qeyri-rəsmi kanallarla qəbul edilir
- Sorğuların izlənilməsi çətindir
- Prioritetlər aydın deyil
- SLA-lar müəyyən edilməyib
- Əməliyyatlar əsasən əl ilə aparılır
- Mərkəzləşdirilmiş görünürlük yoxdur

### Əsas problemlər

| Problem | Təsir | Ciddilik |
| --- | --- | --- |
| **Gecikmələr** | Sorğuların emalı 5-7 iş günü çəkir | 🔴 Yüksək |
| **Şəffaflığın olmaması** | Müştərilər sorğunun statusunu bilmir | 🔴 Yüksək |
| **Əl ilə görülən işlər** | Vaxt aparan, səhvə meyilli əməliyyatlar | 🟠 Orta-yüksək |
| **Məsuliyyət çatışmazlığı** | Kimin nə etdiyi aydın deyil | 🟠 Orta-yüksək |
| **Rəqabət analizlərinin çatışmazlığı** | Məlumat əsaslı qərarlar qəbul edilə bilmir | 🟡 Orta |

## Layihənin məqsədləri

### Əsas hədəflər (SMART)

| Məqsəd | Cari vəziyyət | Hədəf |
| --- | ---: | ---: |
| Sorğuların emal müddətini azaltmaq | 5-7 gün | 30% azalma (3-4 gün) |
| Sorğu statusunun izlənilə bilməsini təmin etmək | 40% | 100% |
| Sorğuları SLA daxilində tamamlamaq | 60% | 90% |
| Əl ilə görülən əməliyyatların payını azaltmaq | — | 50% azalma |
| Dashboard hesabatları hazırlamaq | — | Həftəlik |

## Təklif olunan həll (TO-BE)

### Həllin ümumi görünüşü

1. Sorğunun yaradılması
2. Müvafiq şöbəyə avtomatik yönləndirilməsi
3. Prioritet səviyyəsinin müəyyənləşdirilməsi
4. Məsul işçiyə təyin edilməsi
5. Sorğunun tamamlanması və cavablandırılması
6. Nəticələrin hesabatlarda əks etdirilməsi

### Həllin əsas xüsusiyyətləri

- **Vahid platforma** - Bütün sorğular bir yerdə idarə olunur
- **Avtomatlaşdırılmış iş axınları** - Daxili proseslər avtomatlaşdırılır
- **Real vaxtda görünürlük** - Sorğunun hər mərhələsi izlənilir
- **SLA monitorinqi** - Tapşırıq müddətlərinə avtomatik nəzarət olunur
- **Performans hesabatları** - KPI-lər real vaxtda izlənilir
- **Bildirişlər və eskalasiya** - Avtomatik xatırlatmalar və eskalasiya

## Layihənin əhatə dairəsi (Scope)

### Daxil edilənlər (In Scope)

Daxili sorğuların yaradılması, idarə olunması və izlənilməsi  
İş axınlarının standartlaşdırılması  
Avtomatik yönləndirmə və prioritetləşdirmə  
SLA idarəetməsi  
Performans hesabatları və dashboard  
Bildirişlər sistemi  

### Əhatə dairəsindən kənarda qalanlar (Out of Scope)

Xarici sistemlərlə inteqrasiya (e-poçt, CRM və s.)  
Mobil tətbiq  
Müştəri xidməti portalı (ilk mərhələdə)  
Xərclərin mühasibatlıq sisteminə inteqrasiyası  

## Maraqlı tərəflər (Stakeholders)

### Əsas maraqlı tərəflər

| Maraqlı tərəf | Rolu | Əhəmiyyəti |
| --- | --- | --- |
| **İşçilər (End Users)** | Sorğu yaradanlar | 🔴 Çox yüksək |
| **Departament nümayəndələri** | Sorğuları qəbul edənlər | 🔴 Çox yüksək |
| **İnsan resursları** | Sorğu xidməti provayderi | 🟠 Yüksək |
| **İT şöbəsi** | Sistem idarəçisi | 🟠 Yüksək |
| **Rəhbərlik** | Qərar verənlər | 🟠 Yüksək |
| **Audit və uyğunluq** | Tənzimləyici | 🟡 Orta |

## Əsas tamamlanmış işlər (Key Deliverables)

## Layihə sənədləri

| Mərhələ | Sənəd |
| --- | --- |
| Ümumi baxış | [Rəhbərlər üçün xülasə](./BA_EXECUTIVE_SUMMARY_AZ.md) |
| Metodologiya | [Biznes Analizi Həyat Dövrü Metodologiyası](./BA_LIFECYCLE_METHODOLOGY_AZ.md) |
| Başlanğıc | [Biznes problemi və məqsədlər](./Business%20Problem%20%26%20Objectives.pdf) |
| Başlanğıc | [Maraqlı tərəflərin müəyyənləşdirilməsi və təhlili](./Stakeholder%20Identification%20%26%20Analysis.pdf) |
| Başlanğıc | [Maraqlı tərəflərin xəritəsi](./MIS%20Stakeholder%20Map.png) |
| Başlanğıc | [Risk və fərziyyələr reyestri](./Risk%20%26%20Assumption%20Register.pdf) |
| Analiz və planlaşdırma | [Tələblərin toplanması və kommunikasiya planı](./Elicitation%20%26%20Communication%20Plan.pdf) |
| Analiz və planlaşdırma | [Tələblərin izlənilməsi matrisi](./Requirements%20Traceability%20Matrix.pdf) |
| Analiz və planlaşdırma | [Cari və gələcək vəziyyət](./Current%20%28AS-IS%29%20%26%20Future%20%28TO-BE%29.pdf) |
| Analiz və planlaşdırma | [Cari və gələcək proses xəritəsi](./Current%20vs.%20Future%20State.png) |
| Analiz və planlaşdırma | [Boşluq analizi](./Gap%20Analysis.pdf) |
| Məhsul tələbləri | [İstifadəçi hekayələri və qəbul meyarları](./User%20Stories%20%26%20Acceptance%20Criteria.pdf) |

## Business Analysis-in həyat dövrü

### Mərhələlər və əsas fəaliyyətlər

| Mərhələ | Əsas fəaliyyətlər | Müddət |
| --- | --- | ---: |
| **Başlanğıc (Initiation)** | Problemin və maraqlı tərəflərin müəyyənləşdirilməsi, yüksək səviyyəli tələblərin hazırlanması | 2-3 həftə |
| **Planlaşdırma və analiz** | Tələblərin toplanması, AS-IS və TO-BE analizi, boşluqların müəyyənləşdirilməsi | 3-4 həftə |
| **Həll dizaynı** | Funksional spesifikasiyalar, sistem arxitekturası, User Stories və Acceptance Criteria | 4-5 həftə |
| **Tətbiq** | İnkişaf komandası ilə əməkdaşlıq, dəyişiklik sorğularının idarə olunması və tələblərin dəqiqləşdirilməsi | 8-12 həftə |
| **Sınaq** | UAT planının hazırlanması, test hallarının yoxlanılması və xətaların izlənilməsi | 2-3 həftə |
| **Qiymətləndirmə** | KPI-lərin ölçülməsi, nəticələrin qiymətləndirilməsi və öyrənilmiş dərslər | 1-2 həftə |
