# 📌 GitHub SSH Bağlantısı Kurma ve Repository Clone Etme

## 🛠️ 1. Repository'yi SSH ile Clone Etmeye Çalışın
İlk olarak, SSH kullanarak GitHub repository'nizi bilgisayarınıza klonlamayı deneyin. Bunun için terminal veya Git Bash açarak şu komutu çalıştırın:

```bash
git clone git@github.com:kullanici_adiniz/repo_adiniz.git
```

Eğer daha önce SSH anahtarı oluşturmadıysanız, şu şekilde bir hata alabilirsiniz:

```
Permission denied (publickey).
fatal: Could not read from remote repository.
```

Bu hata, GitHub hesabınızda henüz bir **SSH anahtarı eklenmediğini** gösterir. Şimdi SSH anahtarınızı oluşturup GitHub'a ekleyelim. 🚀

---

## 🔑 2. SSH Anahtarı Oluşturma
Bilgisayarınızda bir SSH anahtarı oluşturmak için aşağıdaki adımları takip edin:

1. **Terminal veya Git Bash'de**  şu komutu çalıştırın:

    ```bash
    ssh-keygen 
    ```
    
   Enter’a basın ve varsayılan konumu kullanarak devam edin.
    
2. **Bir şifre belirleyin (Opsiyonel):**
    
    SSH anahtarınıza ekstra güvenlik için bir şifre belirleyebilirsiniz veya şifresiz bırakmak için **Enter** tuşuna basabilirsiniz.

3. **Anahtar başarıyla oluşturuldu!**
    
    Anahtarınız oluşturulduktan sonra, ilgili dizine gitmek için şu komutu yazın:
    
    ```
    cd ~/.ssh
    ```
4. **Dosyaları listeleyin ve SSH anahtarlarını kontrol edin:**

    ```
    ls 
    ```

---

## 🔗 3. SSH Anahtarını GitHub'a Ekleme
Artık SSH anahtarınızı GitHub hesabınıza eklemelisiniz:

1. Terminalde şu komutu çalıştırarak **public key’i kopyalayın:**
    
    ```bash
    cat id_rsa.pub
    ```
    
    Eğer yukarıda farklı bir isim belirlediyseniz, ona göre değiştirin (`id_github.pub` gibi).

2. Çıkan çıktıyı tamamen **kopyalayın** (örn: `ssh-ed25519 AAAAC3...` ile başlayan uzun bir string).

3. **GitHub’a giriş yapın** ve şu adımları izleyin:
    
    - Sağ üstteki profil resmine tıklayın → **Settings**
    - Sol menüden **SSH and GPG keys** sekmesine gidin.
    - **"New SSH Key"** butonuna tıklayın.
    - **"Title"** kısmına bir isim verin (örneğin: "My Laptop SSH Key").
    - **"Key"** kısmına terminalden kopyaladığınız anahtarı yapıştırın.
    - **"Add SSH Key"** butonuna basın.

---

## ✅ 4. SSH Bağlantınızı Test Edin
Şimdi, GitHub ile bağlantının düzgün çalıştığını test edelim:

```bash
ssh -T git@github.com
```

Eğer her şey doğru çalışıyorsa, şu mesajı almanız gerekir:

```
Hi username! You've successfully authenticated, but GitHub does not provide shell access.
```

Bu mesaj, GitHub hesabınıza SSH ile başarıyla bağlandığınızı gösterir. 🎉

---

## 🚀 5. Repository’yi SSH ile Clone Etme
Şimdi artık SSH bağlantınızı kullanarak repository’nizi clone edebilirsiniz:

```bash
git clone git@github.com:kullanici_adiniz/repo_adiniz.git
```

**Artık GitHub’a her push veya pull işlemi yaptığınızda şifre/token girmenize gerek kalmayacak!** 🎯


###### *Ayrica konuyla ilgili daha ayrıntılı bir video anlatımı için 👉️ [Buraya tıklayabilirsiniz](https://www.youtube.com/watch?v=wPMaggkdlDM)*

