
#Epidemiya simulyasiyaları üçün SİR modelləri

SİR modeli, yoluxucu virusların və xəstəliklərin  modelləştirilməsi
üçün istifadə olunan riyazi modellərdir. SİR modelinin 3 əsas veriləni vardır.

1) S = Suspectible (Şübhəlilər) - Hal hazırda virusa yoluxma ehtimalı olan fərdlərin 
        sayını göstərir
2) İ = İnfected (Yoluxmuş) - Xəstəliyə yoluxmuş aktiv xəstələrin sayını göstərir
3) R = Removed (Bitmiş) - Xəstəlikdən sağalmış və ya ölmüş insanların sayını göstərir

Bundan əlavə, epidemiyanı simulyasiya etmək üçün 2 əlavə faktor vardır.

a) b = İnfection rate (Yoluxma dərəcəsi) - Yoluxma dərəcəsini 0 və 1 arasında
    müəyyən edən kofisent. Modelə input olaraq verilir və seçim istifadəçidən asılıdır

b) y = Recovery rate (Sağalma dərəcəsi) - Sağalma dərəcəsini 0 və 1 arasında 
    müəyyən edən kofisent. 


Əhalinin sayını N ilə işarə edirik və 
                    N = S + İ + R 

Modelin parametrlərinin dəyişimi üçün isə biz 2 ədəd
birinci dərəcəli differensial tənliklərdən istifadə etməliyik


1) d / dT S = -b * İ * S 

Bu ODE , şübhəlilərin yoluxmuş kateqoriyasına keçidini göstərir

2) d / dT İ = b * İ * S - y * İ 

Bu ODE isə yuxarıdakı prosesin əksini, yəni yoluxmuş xəstələrin
bitmiş kateqoriyasına keçidini göstərir