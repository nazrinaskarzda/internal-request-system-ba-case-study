# Biznes Analizi Həyat Dövrü Metodologiyası

## Daxili Sorğu İdarəetmə Sistemi

Bu sənəd Daxili Sorğu İdarəetmə Sistemi layihəsində tətbiq olunan biznes analizi yanaşmasını mərhələlər üzrə təsvir edir. Metodologiya problemin müəyyənləşdirilməsindən nəticələrin qiymətləndirilməsinədək görülən əsas işləri və hazırlanan sənədləri əhatə edir.

## Həyat dövrünün mərhələləri

| Mərhələ | Məqsəd | Əsas nəticə |
| --- | --- | --- |
| 1. Başlanğıc | Problemi, məqsədləri və maraqlı tərəfləri müəyyənləşdirmək | Problem təsviri, əhatə dairəsi, risk və fərziyyələr |
| 2. Planlaşdırma və analiz | Cari prosesi araşdırmaq və tələbləri toplamaq | AS-IS, TO-BE, Gap Analysis və RTM |
| 3. Həll dizaynı | Tələbləri sistem funksiyalarına çevirmək | Proses modelləri, User Stories və Acceptance Criteria |
| 4. Tətbiqə dəstək | Hazırlanma zamanı tələbləri aydınlaşdırmaq | Dəyişiklik qeydləri və yenilənmiş tələblər |
| 5. Sınaq və təsdiqləmə | Həllin tələblərə uyğunluğunu yoxlamaq | Test ssenariləri və UAT nəticələri |
| 6. Qiymətləndirmə | Nəticələri hədəf göstəricilərlə müqayisə etmək | KPI hesabatı və təkmilləşdirmə təklifləri |

## 1. Başlanğıc

### Məqsəd

Layihənin həll etməli olduğu problemi, biznes ehtiyacını, məqsədləri, maraqlı tərəfləri və ilkin əhatə dairəsini müəyyənləşdirmək.

### Problem təsviri

Daxili xidmət sorğuları e-poçt və qeyri-formal əlaqə kanalları vasitəsilə idarə olunur. Mərkəzləşdirilmiş sistem və standart iş axını olmadığı üçün:

- sorğuların emalı 5–7 iş günü çəkir;
- istifadəçilər sorğularının statusunu izləyə bilmirlər;
- SLA müddətlərinə nəzarət çətinləşir;
- sorğuların itməsi və təkrarlanması riski yaranır;
- performans göstəriciləri üzrə vahid hesabat hazırlanmır.

### Maraqlı tərəflərin təhlili

| Maraqlı tərəf | Rolu | Təsir səviyyəsi | Əlaqə yanaşması |
| --- | --- | --- | --- |
| Direktor / CEO | Sponsor | Yüksək | Yaxından idarə et |
| Departament rəhbəri | Product Owner | Yüksək | Yaxından idarə et |
| İT rəhbəri | Texniki rəhbər | Yüksək | Yaxından idarə et |
| İşçilər | Son istifadəçilər | Orta | Məlumatlandır və rəy topla |
| Audit və uyğunluq komandası | Nəzarət tərəfi | Orta | Məlumatlandır və məsləhətləş |
| Maliyyə şöbəsi | Büdcə sahibi | Yüksək | Məmnun saxla və qərarlara cəlb et |

### Əsas fərziyyələr

| Fərziyyə | Ehtimal olunan təsir | İdarəetmə yanaşması |
| --- | --- | --- |
| Maraqlı tərəflər layihəyə lazımi dəstəyi verəcək | Yüksək | Müntəzəm görüşlər və qərar qeydləri |
| Büdcə 200 000 AZN həddini keçməyəcək | Yüksək | Əhatə dairəsinə və xərclərə nəzarət |
| İlk mərhələdə xarici sistem inteqrasiyasına ehtiyac olmayacaq | Orta | Gələcək inteqrasiyalar üçün çevik arxitektura |
| Sistemdən 200-dən çox işçi istifadə edəcək | Yüksək | Təlim və dəyişikliklərin idarə edilməsi planı |

### Əsas risklər

| Risk | Ehtimal | Təsir | Qarşı tədbir |
| --- | --- | --- | --- |
| Maraqlı tərəflərin iştirakının azalması | Orta | Yüksək | Müntəzəm status görüşləri |
| Tələblərin dəyişməsi | Yüksək | Orta | Dəyişikliklərin idarə edilməsi prosesi |
| İstifadəçilərin sistemi mənimsəməməsi | Orta | Yüksək | Erkən cəlbetmə və təlim |
| Texniki mürəkkəblik | Orta | Orta | Prototip və texniki uyğunluq yoxlaması |

### SMART məqsədlər

| Göstərici | Cari vəziyyət | Hədəf |
| --- | ---: | ---: |
| Sorğuların emal müddəti | 5–7 iş günü | 3–4 iş günü |
| Sorğuların izlənilə bilməsi | 40% | 100% |
| SLA uyğunluğu | 60% | 90% |
| Əl əməliyyatlarının payı | — | 50% azalma |
| Sistemin əlçatanlığı | — | Ən azı 99% |

MVP-nin üç ay, tam tətbiqin isə altı ay ərzində hazırlanması planlaşdırılır.

### Əhatə dairəsi

**Daxildir:**

- sorğuların yaradılması və izlənilməsi;
- avtomatik iş axınları və yönləndirmə;
- SLA idarəetməsi;
- performans hesabatları;
- bildirişlər sistemi;
- audit tarixçəsi.

**Daxil deyil:**

- xarici sistemlərlə inteqrasiya;
- ilk mərhələdə mobil tətbiq;
- əməkhaqqı sistemi ilə inteqrasiya;
- müştəri xidməti portalı.

### Mərhələnin nəticələri

- Business Problem & Objectives
- Stakeholder Identification & Analysis
- Assumptions & Risk Log
- High-Level Scope Statement
- Success Criteria

## 2. Planlaşdırma və analiz

### Məqsəd

Cari və gələcək vəziyyəti təhlil etmək, aradakı boşluqları müəyyənləşdirmək və biznes tələblərini sənədləşdirmək.

### Tələblərin toplanması üsulları

| Üsul | İştirakçılar | Məqsəd |
| --- | --- | --- |
| Müsahibə | Departament rəhbərləri və əsas istifadəçilər | Biznes ehtiyaclarını və problemləri anlamaq |
| İş sessiyası | Proses sahibləri və işçilər | Tələbləri birlikdə müəyyənləşdirmək və prioritetləşdirmək |
| Sənəd təhlili | Biznes analitiki | Mövcud prosedurları, formaları və yazışmaları araşdırmaq |
| Müşahidə | Son istifadəçilər | Cari iş axınını real şəraitdə izləmək |
| Sorğu | Geniş istifadəçi qrupu | Gözləntiləri və məmnuniyyət səviyyəsini ölçmək |

### Cari proses — AS-IS

1. İşçi sorğunu e-poçt vasitəsilə göndərir.
2. Sorğu müvafiq cədvəldə əl ilə qeyd olunur.
3. Departament rəhbəri məsul şəxsi müəyyənləşdirir.
4. Məsul şəxs əlavə məlumat toplayır.
5. Sorğu icra edilir.
6. Nəticə e-poçt vasitəsilə işçiyə bildirilir.

Bu proses orta hesabla 5–7 iş günü çəkir. Əsas problemlər sorğuların itməsi, təkrarlanması, prioritetlərin qeyri-müəyyənliyi və statusun görünməməsidir.

### Gələcək proses — TO-BE

1. İşçi sorğunu veb-portalda yaradır.
2. Sistem sorğunu qaydalara əsasən avtomatik yönləndirir.
3. Məsul şəxs bildiriş alır və sorğunu icraya götürür.
4. Status dəyişiklikləri sistemdə qeydə alınır.
5. SLA riski yarandıqda sistem xatırlatma və eskalasiya göndərir.
6. Sorğu tamamlandıqda işçiyə avtomatik bildiriş göndərilir.

Hədəf emal müddəti 3–4 iş günüdür. Sorğuların statusu real vaxt rejimində görünür və performans məlumatları avtomatik toplanır.

### Boşluq analizi

| Sahə | AS-IS | TO-BE | Tələb olunan dəyişiklik |
| --- | --- | --- | --- |
| Sorğunun yaradılması | E-poçt | Veb-forma | İstifadəçi portalı |
| Yönləndirmə | Əl ilə | Avtomatik | İş axını qaydaları |
| Prioritetləşdirmə | Qeyri-formal | Qayda əsaslı | Biznes qaydaları |
| Statusun izlənilməsi | Cədvəl | Real vaxt rejimi | Mərkəzləşdirilmiş məlumat bazası |
| SLA nəzarəti | Əl ilə | Avtomatik | SLA və eskalasiya mexanizmi |
| Hesabatlılıq | Əl ilə hazırlanan hesabat | İdarəetmə paneli | Analitika modulu |
| Audit tarixçəsi | Mövcud deyil | Tam qeydiyyat | Audit jurnalı |

### Tələblərin sənədləşdirilməsi

Tələblər üç kateqoriya üzrə qruplaşdırılır:

- **Biznes tələbləri:** həllin hansı biznes nəticəsini təmin etməli olduğunu göstərir.
- **Funksional tələblər:** sistemin yerinə yetirməli olduğu funksiyaları təsvir edir.
- **Qeyri-funksional tələblər:** performans, təhlükəsizlik, istifadə rahatlığı və əlçatanlıq meyarlarını müəyyənləşdirir.

Nümunə tələblər:

| ID | Tələb | Prioritet | Yoxlama meyarı |
| --- | --- | --- | --- |
| BR-001 | Bütün daxili sorğular vahid platformada idarə olunmalıdır | Kritik | Sorğular sistemdə yaradıla və izlənilə bilir |
| BR-002 | İstifadəçi sorğunun cari statusunu görə bilməlidir | Yüksək | Status idarəetmə panelində göstərilir |
| FR-001 | Sistem sorğu yaratmaq üçün standart forma təqdim etməlidir | Yüksək | Məcburi sahələr yoxlanılır və sorğu ID-si yaradılır |
| FR-002 | Sistem sorğuları kateqoriya üzrə avtomatik yönləndirməlidir | Yüksək | Sorğu uyğun komandaya təyin edilir |
| NFR-001 | Əsas səhifələr 2 saniyədən gec açılmamalıdır | Yüksək | Performans sınağı tələbi təsdiqləyir |
| NFR-002 | Giriş rol əsaslı icazələrlə qorunmalıdır | Kritik | İcazəsiz giriş bloklanır və qeydə alınır |

### Tələblərin izlənilməsi

Requirements Traceability Matrix hər bir tələbi onun mənbəyi, əlaqəli funksiyası, test ssenarisi və statusu ilə əlaqələndirir. Bu yanaşma tələblərin itirilməsinin qarşısını alır və dəyişikliklərin təsirini izləməyə imkan verir.

### Mərhələnin nəticələri

- Elicitation & Communication Plan
- Current AS-IS & Future TO-BE
- Gap Analysis
- Business və System Requirements
- Requirements Traceability Matrix

## 3. Həll dizaynı

### Məqsəd

Təsdiqlənmiş tələbləri sistem funksiyalarına, proses axınlarına və istifadəçi ssenarilərinə çevirmək.

### Əsas istifadəçi rolları

| Rol | Əsas əməliyyatlar |
| --- | --- |
| İşçi | Sorğu yaratmaq, statusu izləmək və nəticəni görmək |
| Menecer | Sorğunu təsdiqləmək və prioriteti idarə etmək |
| Sorğunu icra edən şəxs | Sorğunu qəbul etmək, yeniləmək və tamamlamaq |
| Sistem administratoru | İstifadəçiləri, rolları və iş axını qaydalarını idarə etmək |

### Əsas məlumat obyektləri

| Obyekt | Əsas məlumatlar |
| --- | --- |
| Employee | ID, ad, e-poçt, departament və rol |
| Request | ID, növ, təsvir, prioritet, status, son tarix və məsul şəxs |
| Request Status | Statusun adı və təsviri |
| Comment | Sorğu, müəllif, mətn və tarix |
| Attachment | Sorğu, fayl yolu, ölçü və yüklənmə tarixi |

### User Stories nümunələri

**Sorğunun yaradılması**

> Bir işçi kimi, ehtiyac duyduğum dəstəyi almaq üçün xidmət sorğusu yaratmaq və göndərmək istəyirəm.

Qəbul meyarları:

- forma sorğunun növü, təsviri, prioriteti və əlavələri qəbul edir;
- məcburi sahələr göndərilmədən əvvəl yoxlanılır;
- uğurlu göndərişdən sonra unikal sorğu nömrəsi göstərilir;
- istifadəçiyə təsdiq bildirişi göndərilir.

**Sorğunun statusunun izlənilməsi**

> Bir işçi kimi, həll müddətini təxmin edə bilmək üçün sorğumun cari statusunu görmək istəyirəm.

Qəbul meyarları:

- istifadəçi yalnız öz sorğularını görə bilir;
- hər sorğu üzrə status, yaradılma tarixi və məsul şəxs göstərilir;
- siyahı statusa, tarixə və prioritetə görə süzülə bilir;
- sorğu nömrəsi üzrə axtarış mümkündür.

**Avtomatik bildirişlərin alınması**

> Sorğunu icra edən şəxs kimi, yeni təyinatları gecikdirməmək üçün avtomatik bildiriş almaq istəyirəm.

Qəbul meyarları:

- sorğu təyin edilən kimi bildiriş göndərilir;
- bildirişdə sorğunun nömrəsi, prioriteti və son tarixi göstərilir;
- istifadəçi bildiriş seçimlərini idarə edə bilir.

### Əsas biznes qaydaları

| Qayda | Təsvir |
| --- | --- |
| Prioritetin təyin edilməsi | Prioritet sorğunun növü, biznes təsiri və təcililik səviyyəsinə əsasən müəyyənləşdirilir |
| SLA hesablanması | Hər sorğu növü üçün ayrıca cavab və həll müddəti tətbiq olunur |
| Eskalasiya | SLA müddətinin 75%-i keçdikdə məsul şəxsə və menecerə bildiriş göndərilir |
| Avtomatik təyinat | Sorğu kateqoriya, iş yükü və səlahiyyət əsasında uyğun icraçıya yönləndirilir |
| Dublikatların yoxlanılması | Oxşar məzmunlu sorğular birləşdirilməzdən əvvəl istifadəçiyə göstərilir |
| Təsdiq axını | Təsdiq tələb edən sorğular icradan əvvəl müvafiq menecerə yönləndirilir |

### Mərhələnin nəticələri

- User Stories & Acceptance Criteria
- Functional və Non-Functional Requirements
- Use Case və proses modelləri
- Məlumat modeli
- Business Rules

## 4. Tətbiqə dəstək

### Məqsəd

Hazırlanma zamanı tələblərin düzgün başa düşülməsini təmin etmək və təsdiqlənmiş əhatə dairəsini qorumaq.

Əsas fəaliyyətlər:

- komandanın suallarını cavablandırmaq və tələbləri aydınlaşdırmaq;
- dəyişiklik sorğularını qeydə almaq və təsirini qiymətləndirmək;
- backlog elementlərini prioritetləşdirmək;
- həllin biznes qaydalarına uyğunluğunu yoxlamaq;
- sənədləri qəbul edilmiş dəyişikliklərə uyğun yeniləmək.

## 5. Sınaq və təsdiqləmə

### Məqsəd

Hazırlanmış həllin biznes və sistem tələblərinə cavab verdiyini yoxlamaq.

Əsas fəaliyyətlər:

- qəbul meyarlarına əsasən test ssenarilərinin hazırlanması;
- müsbət və mənfi istifadə ssenarilərinin yoxlanılması;
- User Acceptance Testing prosesinin planlaşdırılması;
- aşkarlanan uyğunsuzluqların tələblərlə əlaqələndirilməsi;
- biznes tərəfinin yekun təsdiqinin alınması.

## 6. Qiymətləndirmə

### Məqsəd

Tətbiqdən sonra nəticələri ilkin məqsədlər və KPI-larla müqayisə etmək.

İzlənilən əsas göstəricilər:

- sorğuların orta emal müddəti;
- SLA daxilində tamamlanan sorğuların payı;
- açıq və gecikmiş sorğuların sayı;
- avtomatik yönləndirilən sorğuların payı;
- istifadəçi məmnuniyyəti;
- sistemin əlçatanlığı.

Qiymətləndirmə nəticəsində təkmilləşdirmə imkanları müəyyənləşdirilir, backlog yenilənir və növbəti mərhələ üçün prioritetlər formalaşdırılır.

## İstifadə olunan alətlər və şablonlar

| Alət | İstifadə məqsədi |
| --- | --- |
| Google Docs | Biznes və məhsul sənədlərinin hazırlanması |
| Google Sheets | Tələblərin, risklərin və izləmə məlumatlarının idarə edilməsi |
| Lucidchart | Proses və maraqlı tərəf diaqramlarının hazırlanması |

Əsas şablonlar:

- User Story və Acceptance Criteria;
- Requirements Traceability Matrix;
- Risk və Assumption Register;
- Elicitation & Communication Plan;
- Change Request Log;
- UAT ssenariləri.

---

**Hazırlayan:** Nazrin Askarzada  
**Rol:** Product Owner / Business Analyst

> Bu sənəd portfolio məqsədilə hazırlanmış konseptual case study-nin bir hissəsidir.
