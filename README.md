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
| Başlanğıc | [Business Problem & Objectives](https://docs.google.com/document/d/1vJBJdLolPeqADzZ7iQUlhgdgFIsihq_z7T1QdHDo3w0/edit?usp=drivesdk) |
| Başlanğıc | [Stakeholder Identification & Analysis](https://docs.google.com/spreadsheets/d/1dRbUta5tM175rLT0mKaDoJ-3qG-udGWILqVc2Z5fmys/edit?usp=drivesdk) |
| Başlanğıc | [MIS Stakeholder Map](https://docs.google.com/spreadsheets/d/1dRbUta5tM175rLT0mKaDoJ-3qG-udGWILqVc2Z5fmys/edit?usp=drivesdk) |
| Başlanğıc | [Risk & Assumption Register](https://docs.google.com/spreadsheets/d/1_PL97gybJtXfxYYvVc2LZZFk2Ly5DT0T9lYLy699_co/edit?usp=drivesdk) |
| Analiz və planlaşdırma | [Elicitation & Communication Plan](https://docs.google.com/spreadsheets/d/1qXvmfMIY11Hd1QUBhcX1xuNw7rSPrKtQ6tVTYNQjdf0/edit?usp=drivesdk) |
| Analiz və planlaşdırma | [Requirements Traceability Matrix](https://docs.google.com/spreadsheets/d/154nLduUGugK5EDZolFAqD4EEjvxUmKNOovvY8wq8F7g/edit?usp=drivesdk) |
| Analiz və planlaşdırma | [Current (AS-IS) & Future (TO-BE)](https://docs.google.com/document/d/1w_yTvtuZTs7NiVZ9wtQnXLjC6UEiKtDIkyEYZHXJ4Ec/edit?usp=drivesdk) |
| Analiz və planlaşdırma | [Current vs. Future State Modelling](https://docs.google.com/document/d/1w_yTvtuZTs7NiVZ9wtQnXLjC6UEiKtDIkyEYZHXJ4Ec/edit?usp=drivesdk) |
| Analiz və planlaşdırma | [Gap Analysis](https://docs.google.com/document/d/1VpKm00FRRXGfYzLqa50KqN752f3t56T-E0BEtGwn1Ho/edit?usp=drivesdk) |
| Məhsul tələbləri | [User pencils & Acceptance Criteria](https://docs.google.com/document/d/1Mup-m4dvQ-IEn5T28pIjEU3CPKco08hC57G8ZRiu9Qw/edit?usp=drivesdk) |
| Məhsul tələbləri | [Request Creation - Functional Specification](https://docs.google.com/document/d/14Wn3iZ9D8AhY0x1wI1bv_ogWl7U2JYA6rnx8iIN2uUA/edit?usp=drivesdk) |
| Məlumatların modelləşdirilməsi | [Data Dictionary Overview](https://docs.google.com/document/d/1BwRAsoK0T3DBYsKBtIChU3EMjj5zqS2GDDWSOZN7wzs/edit?usp=drivesdk) |
| Məlumatların modelləşdirilməsi | [Data Dictionary](https://docs.google.com/spreadsheets/d/1HE84l3joOsPNKrL-9W_Ej8OTIH0cPS36Io9k1_DnHv8/edit?usp=drivesdk) |
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
