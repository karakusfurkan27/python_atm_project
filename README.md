### README: ATM Sistemi

#### Proje Açıklaması

Bu proje, basit bir ATM (Bankamatik) sistemi simülasyonu yapmaktadır. Kullanıcı, bankamatik üzerinden bakiye kontrolü yapabilir, para yatırabilir, para çekebilir ve sistemi sonlandırabilir. Proje, Python programlama dili ile yazılmıştır ve kullanıcıyla metin tabanlı bir arayüz üzerinden etkileşim kurar.

---

#### Dosya ve Sınıf Açıklamaları

**1. `BankAccount` Sınıfı**  
Bu sınıf, bir banka hesabını temsil eder ve aşağıdaki özellikleri sağlar:  
- **`__init__(owner, balance=0)`**: Hesap sahibi ve başlangıç bakiyesi tanımlanır. Varsayılan bakiye `0 TL`'dir.
- **`deposit(amount)`**: Hesaba para yatırmayı sağlar. Yatırılan miktar pozitif olmalıdır.
- **`withdraw(amount)`**: Hesaptan para çekmeyi sağlar. Çekilecek miktar, mevcut bakiyeden fazla olmamalı ve pozitif bir değer olmalıdır.
- **`check_balance()`**: Hesabın mevcut bakiyesini ekrana yazdırır.

**2. `atm_menu` Fonksiyonu**  
Kullanıcıya bankamatik menüsünü ekrana yazdırır. Menünün içeriği şunlardır:  
- Bakiye Kontrolü
- Para Yatırma
- Para Çekme
- Çıkış

**3. `atm` Fonksiyonu**  
ATM sisteminin ana işleyişini yönetir. `BankAccount` sınıfını kullanarak kullanıcı işlemlerini gerçekleştirir ve seçimlere göre uygun fonksiyonları çağırır.

---

#### Kullanım

1. **Kodun Çalıştırılması**  
   Bu projeyi çalıştırmak için aşağıdaki adımları takip edin:  
   - Python 3 yüklü olduğundan emin olun.  
   - Kod dosyasını bir Python IDE veya terminal üzerinden çalıştırın.  

   ```bash
   python atm.py
   ```

2. **ATM Menüsü**  
   Kod çalıştırıldığında kullanıcı bir ATM menüsü görecektir. Kullanıcı, belirtilen numaralarla seçim yaparak işlemlerini gerçekleştirebilir:  
   - **1**: Mevcut bakiyeyi kontrol eder.  
   - **2**: Belirtilen bir miktar kadar para yatırır.  
   - **3**: Belirtilen bir miktar kadar para çeker.  
   - **4**: Sistemden çıkış yapar.  

3. **Örnek Kullanım**  
   - Para yatırma seçeneğini seçip `100` miktarını girerseniz:  
     ```
     100 TL yatırıldı. Yeni bakiye: 100 TL
     ```
   - Para çekme seçeneğini seçip `50` miktarını girerseniz:  
     ```
     50 TL çekildi. Yeni bakiye: 50 TL
     ```
   - Bakiye kontrolü yaparsanız:  
     ```
     Mevcut bakiye: 50 TL
     ```

---

#### Gereksinimler

- **Python 3.x**  
- Herhangi bir ek kütüphane yüklenmesine gerek yoktur.

---

#### Notlar

- Bu ATM sistemi, gerçek bir bankacılık sistemi değildir. Basit bir eğitim amaçlı simülasyondur.  
- Kullanıcı, negatif miktarlar girerse veya çekilecek miktar bakiyeden büyük olursa sistem uygun hata mesajlarını ekrana yazdırır.  

---

#### Geliştirme İmkânları

Proje daha da geliştirilebilir. Örneğin:  
- Birden fazla kullanıcı için destek eklenebilir.  
- Hesap hareketlerini kayıt eden bir log sistemi eklenebilir.  
- Grafiksel bir kullanıcı arayüzü (GUI) geliştirilebilir.
