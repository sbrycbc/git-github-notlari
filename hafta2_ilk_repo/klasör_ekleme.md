## **GitHub Reposuna Klasör Ekleme Adımları**

### 1. GitHub Reponuzu Clone Etme (Bilgisayarınıza İndirme)
İlk olarak, GitHub'daki repository’nizi bilgisayarınıza indirmeniz gerekiyor.

1. GitHub'da ilgili repository’nizi açın.
2. Sağ üst köşede **Code** butonuna tıklayın ve oradan **SSH** linkini kopyalayın (örneğin: `git clone git@github.com:kullanici_adiniz/repo_adiniz.git`).
3. Bilgisayarınızda **Git Bash** (veya terminal) açın ve şu komutu girerek repository’yi bilgisayarınıza indirin:

    ```bash
    git clone git@github.com:kullanici_adiniz/repo_adiniz.git
    ```

    Bu komut, repository’nizi bilgisayarınıza indirecek. Sonrasında, terminalde repository'nizin klasörüne gitmek için şu komutu kullanın:

    ```bash
    cd repo_adiniz
    ```

### 2. Yeni Klasör ve Dosya Oluşturma
Şimdi repository'niz bilgisayarınızda yerel olarak mevcut. Bu dizine yeni bir klasör oluşturabilirsiniz:

1. Yeni bir klasör oluşturmak için şu komutu kullanın:

    ```bash
    mkdir images
    ```

    Bu komut, `images` adında yeni bir klasör oluşturur.

2. Klasöre fotograflari direkt olarak images klasörüne sürükleyip bırakabilirsiniz

   

### 3. Değişiklikleri Git ile Kaydetme
Yeni klasör ve dosyanız repository’ye eklenmiş oldu. Şimdi bu değişiklikleri Git ile kaydetmeniz gerekiyor.

1. Öncelikle, eklediğiniz dosyayı git'e ekleyin:

    ```bash
    git add images/*
    ```

    (Eğer tüm değişiklikleri eklemek isterseniz, `git add .` komutunu kullanabilirsiniz.)

### 4. Commit Yapma
Değişiklikleri commit etmek için şu komutu kullanın:
 
```bash
git commit -m "Add 'images' folder with placeholder file"
 ```

### GitHub’a Yükleme (Push)
Son olarak, değişikliklerinizi GitHub’a göndermek için şu komutu kullanın:
 
```bash
git push origin main
```
