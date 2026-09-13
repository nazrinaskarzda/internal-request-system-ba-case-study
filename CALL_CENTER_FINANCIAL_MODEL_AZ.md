# Çağrı mərkəzində AI tətbiqi — maliyyə modeli

Bu sənəddə çağrıların süni intellekt (AI) vasitəsilə avtomatlaşdırılmasının maliyyə təsiri pessimist, realist və optimist ssenarilər üzrə qiymətləndirilir.

## Modelin məqsədi

Model AI üçün uyğun zənglərin avtomatlaşdırılmasının operator iş yükünə, aylıq xərclərə və investisiyanın geriödəmə müddətinə təsirini hesablayır.

## Əsas fərziyyələr

| Göstərici | Dəyər |
| --- | ---: |
| Aylıq zəng sayı | 120 000 |
| Operatorla orta zəng müddəti | 6 dəqiqə |
| AI ilə orta zəng müddəti | 3,5 dəqiqə |
| AI üçün uyğun zənglərin payı | 65% |
| İş rejimi | 8 saat/gün, 22 gün/ay |
| Məşğulluq səviyyəsi | 75% |
| Bir operatorun aylıq xərci | 1 500 AZN |
| Telefoniya xərci | 0,02 AZN/dəqiqə |
| AI-nin dəyişən xərci | 0,10 AZN/dəqiqə |
| AI platformasının aylıq sabit xərci | 4 000 AZN |
| Birdəfəlik tətbiq xərci | 36 000 AZN |
| Amortizasiya müddəti | 24 ay |

Bu fərziyyələrə əsasən bir operatorun aylıq effektiv iş tutumu 7 920 dəqiqə, AI-sız baza operator ehtiyacı isə 90,91 FTE-dir.

## Ssenari parametrləri

| Ssenari | AI tərəfindən həll olunma səviyyəsi | Qənaətin reallaşma payı |
| --- | ---: | ---: |
| Pessimist | 40% | 40% |
| **Realist** | **60%** | **75%** |
| Optimist | 78% | 95% |

## Hesablama qaydası

| Hesablama | Formula |
| --- | --- |
| AI-yə yönləndirilən zənglər | Aylıq zəng sayı × uyğun zənglərin payı × AI tərəfindən həll olunma səviyyəsi |
| İş yükünün azalması | AI-yə yönləndirilən zənglər ÷ ümumi zəng sayı |
| Potensial FTE qənaəti | Baza FTE × iş yükünün azalması |
| Reallaşdırılan FTE qənaəti | Potensial FTE qənaəti × reallaşma payı |
| Operator xərclərinə qənaət | Reallaşdırılan FTE qənaəti × bir operatorun aylıq xərci |
| Telefoniya qənaəti | AI zəngləri × vaxt fərqi × dəqiqəlik telefoniya xərci |
| AI-nin dəyişən xərci | AI zəngləri × AI zəng müddəti × dəqiqəlik AI xərci |
| Aylıq xalis fayda | Operator qənaəti + telefoniya qənaəti − AI xərcləri − amortizasiya |

## Əməliyyat nəticələri

| Göstərici | Pessimist | **Realist** | Optimist |
| --- | ---: | ---: | ---: |
| AI-yə yönləndirilən aylıq zəng sayı | 31 200 | **46 800** | 60 840 |
| İş yükünün azalması | 26% | **39%** | 50,7% |
| Potensial FTE qənaəti | 23,64 | **35,45** | 46,09 |
| Reallaşdırılan FTE qənaəti | 9,45 | **26,59** | 43,79 |

## Aylıq maliyyə nəticələri

| Maddə | Pessimist | **Realist** | Optimist |
| --- | ---: | ---: | ---: |
| Operator xərclərinə qənaət | +14 182 AZN | **+39 886 AZN** | +65 680 AZN |
| Telefoniya xərclərinə qənaət | +1 560 AZN | **+2 340 AZN** | +3 042 AZN |
| AI-nin dəyişən xərci | −10 920 AZN | **−16 380 AZN** | −21 294 AZN |
| AI platformasının sabit xərci | −4 000 AZN | **−4 000 AZN** | −4 000 AZN |
| Tətbiq xərcinin amortizasiyası | −1 500 AZN | **−1 500 AZN** | −1 500 AZN |
| **Xalis aylıq fayda** | **−678 AZN** | **20 346 AZN** | **41 928 AZN** |

## İnvestisiya göstəriciləri

| Göstərici | Pessimist | **Realist** | Optimist |
| --- | ---: | ---: | ---: |
| İllik xalis fayda | −8 138 AZN | **244 156 AZN** | 503 131 AZN |
| Model üzrə illik ROI | −22,61% | **678,21%** | 1 397,58% |
| Geriödəmə müddəti | Geri ödənmir | **1,77 ay** | 0,86 ay |
| Nəticə | Zərərli | **Mənfəətli** | Mənfəətli |

> ROI modeldə illik xalis faydanın 36 000 AZN məbləğində birdəfəlik tətbiq xərcinə nisbəti kimi hesablanır.

## Ssenarilər üzrə təhlil

### Pessimist ssenari

AI ayda 31 200 zəngi idarə edir və iş yükünü 26% azaldır. Reallaşdırılan qənaət 9,45 FTE ilə məhdudlaşdığı üçün aylıq nəticə 678 AZN zərərdir. Bu ssenaridə investisiya geri ödənmir.

### Realist ssenari

AI ayda 46 800 zəngi idarə edir və iş yükünü 39% azaldır. 26,59 FTE həcmində reallaşdırılan qənaət nəticəsində aylıq xalis fayda 20 346 AZN, illik xalis fayda isə 244 156 AZN təşkil edir. Birdəfəlik tətbiq xərci təxminən 1,77 aya geri ödənir.

### Optimist ssenari

AI ayda 60 840 zəngi idarə edir və iş yükünü 50,7% azaldır. Reallaşdırılan qənaət 43,79 FTE-yə çatır. Aylıq xalis fayda 41 928 AZN, illik xalis fayda isə 503 131 AZN-dir. İnvestisiyanın geriödəmə müddəti 0,86 aydır.

## Nəticə

- Pessimist ssenari maliyyə baxımından sərfəli deyil.
- Realist ssenari müsbət maliyyə nəticəsi verir və əsas qərar ssenarisi kimi istifadə oluna bilər.
- Optimist ssenari yüksək gəlirlilik göstərir, lakin AI-nin uyğun zənglərin 78%-ni həll etməsi və potensial qənaətin 95%-nin reallaşması şərtindən asılıdır.
- Tətbiq qərarından əvvəl AI tərəfindən həll olunma səviyyəsi və faktiki FTE qənaəti pilot mərhələdə yoxlanmalıdır.

## Fayllar

- [Layihənin README faylı](./CALL_CENTER_AI_README_AZ.md)
- [İnteraktiv maliyyə modelini aç](https://docs.google.com/spreadsheets/d/1GB4fukYxZQ1f7sWiT2pOoza5KaAzwR2Hv6CwofCF72I/edit?gid=1978403608#gid=1978403608)
- [PDF hesabatına bax](./Call_Center_AI_Business_Case.pdf)

---

**Hazırlayan:** Nazrin Askarzada  
**Rol:** Product Growth Analyst

> Qeyd: Hesablamalar model fərziyyələrinə əsaslanır. Faktiki nəticələr zəng strukturu, AI performansı və qənaətin reallaşma səviyyəsindən asılı olaraq dəyişə bilər.
