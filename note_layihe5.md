# Böyük Britaniya Elektron Ticarət Məlumatlarında Gəlir Təhlili və Müştəri Səviyyəsində Aqreqasiya

## Metodologiya
- Dataset: data.csv (541909 sətir, 8 sütun, encoding='ISO-8859-1')
- Ləğv edilmiş sifarişlər (Faktura No "C" ilə başlayan, 9288 sətir) ayrıca saxlanıldı
- Müştəri səviyyəli təhlil üçün CustomerID-si boş olan 135080 sətir çıxarıldı
- Mənfi Miqdarlı (qaytarım) 8905 sətir ayrıca qeyd edildi
- Gəlir sütunu yaradıldı: Miqdar x Vahid Qiymət
- Müştəri ID və Ölkə üzrə ümumiləşdirmə aparıldı
- InvoiceDate-dən ay çıxarılıb, aylıq gəlir trendi hesablandı
- Faktura başına unikal məhsul sayı ilə "səbət ölçüsü" hesablandı
- Ən yaxşı 10 ölkənin sütun qrafiki və qaytarma dərəcəsi qrafiki seaborn ilə çəkildi

## Əsas Tapıntılar
- Ümumi xalis gəlir: 8300065.81 GBP
- United Kingdom ümumi gəlirin 81.54%-ni təşkil edir
- Ən yüksək gəlirli ay: Noyabr 2011 (1132407.74 GBP) - Milad effekti
- Ən yaxşı müştəri (ID 14646) 279489.02 GBP gəlir gətirib
- Ən çox satılan məhsul: WORLD WAR 2 GLIDERS ASSTD DESIGNS
- Ləğv edilmiş sifarişlərin faizi: 1.71%
- Qaytarım sətirlərinin faizi: 2.19%
- Ən yüksək qaytarma nisbətinə malik ölkələr: Czech Republic (60%), Malta (50%)
- Ən böyük səbət ölçüsünə malik ölkə: RSA (58 unikal məhsul/faktura)
