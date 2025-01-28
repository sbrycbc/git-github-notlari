## **Adım 1: Git'i Kurma**

### **Windows için Kurulum**
1. [Git resmi web sitesine](https://git-scm.com) gidin.
2. "Download for Windows" seçeneğini tıklayın.
3. İndirilen kurulum dosyasını çalıştırın ve yönergeleri izleyin.
   - Varsayılan ayarlarla ilerleyebilirsiniz.
4. Kurulum tamamlandıktan sonra terminali açıp şu komutla kontrol edin:
   ```bash
   git --version
   ```
   Eğer bir sürüm numarası görüyorsanız, kurulum başarılıdır.


### **macOS için Kurulum**
1. Terminali açın.
2. Git'in kurulu olup olmadığını kontrol edin:
   ```bash
   git --version
   ```
   - Eğer kurulu değilse, terminal size Xcode Command Line Tools'u yüklemek isteyip istemediğinizi soracaktır. "Evet" deyin ve kurulumun tamamlanmasını bekleyin.

### **Linux için Kurulum**
- Debian/Ubuntu tabanlı sistemler için:
  ```bash
  sudo apt update
  sudo apt install git
  ```
- Fedora tabanlı sistemler için:
  ```bash
  sudo dnf install git
  ```
- Kontrol etmek için:
  ```bash
  git --version
  ```

## **Adım 2: Git Ayarları**
Git'i ilk kez kullanmadan önce kullanıcı bilgilerinizi ayarlamanız gerekiyor:

1. Kullanıcı adınızı ayarlayın:
   ```bash
   git config --global user.name "Adınız"
   ```
2. E-posta adresinizi ayarlayın:
   ```bash
   git config --global user.email "email@adresiniz.com"
   ```
3. Ayarları kontrol edin:
   ```bash
   git config --list
   ```
   Bu komut, ayarlarınızı görüntüler.

## **Adım 3: Terminal Nedir ve Nasıl Kullanılır?**
### **Terminal Nedir?**
Terminal, bilgisayarınıza komutlar yazarak işlemler yapmanızı sağlayan bir araçtır. 

### **Sık Kullanılan Terminal Komutları**
| Komut          | Açıklama                                     |
|----------------|----------------------------------------------|
| `pwd`          | Geçerli çalışma dizinini gösterir.           |
| `ls`           | Klasör içindeki dosyaları listeler.          |
| `cd <klasör>`  | Belirtilen klasöre gider.                    |
| `mkdir <isim>` | Yeni bir klasör oluşturur.                   |
| `rm <dosya>`   | Bir dosyayı siler.                           |

#### **Kullanim Örnekleri**
1. **Yeni bir klasör oluşturmak ve içine gitme komutlari:**
   ```bash
   mkdir ilk_proje
   cd ilk_proje
   ```
2. **İçeride bir dosya oluşturmak:**

  -  **Eğer dosya içine başlangıçta bir metin eklemek istiyorsanız:**

  a. Metin ekleme:
   ```bash
     echo "Merhaba Git" > merhaba.txt
   ```

  b. İçeriği kontrol etme:
   ```bash
     cat  merhaba.txt
   ```
 c. Çıktı:
   ```bash
     Merhaba Git
   ```

   -  **Eğer sadece boş bir dosya oluşturmak istiyorsanız:**

  ```bash
     touch merhaba.txt
  ```
3. **Dosya Silme:**

  a. Tek bir dosya silmek:  

  ```bash
     rm dosya_adi
   ```
   b. Birden fazla dosya silmek:

   ```bash
     rm dosya_adi dosya2_adi
   ```

   c. Tüm dosyalari silmek:

   ```bash
     rm *
   ```

   d. Dikkat edilmesi gereken noktalar:

⚠️⚠️ Bir dosyayı rm ile sildiğinde, bu işlem geri alınamaz. Bu yüzden emin olmadan kullanilmamasi gerekiyor.⚠️⚠️

4. **Klasör Silme:**

- Bir klasörü ve içindeki tüm dosyaları silmek:

 ```bash
     rm -r dosya_adi
   ```
---

## **Adım 4: İlk Depo Oluşturma ve Kontrol**
1. Yeni bir Git deposu başlatın:
   ```bash
   git init
   ```
   Bu komut, mevcut klasörü bir Git deposuna dönüştürür.

2. Yeni dosyayı ekleyin:
   ```bash
   git add merhaba.txt
   ```

3. Değişiklikleri kaydedin:
   ```bash
   git commit -m "İlk commit"
   ```

4. Durumu kontrol edin:
   ```bash
   git status
   ```
5. Olusturulan gizli git dosyasini görmek icin:
   ```bash
   ls -a
   ```