## 📌 2. Hafta Ödevi: GitHub’da Dünya Mutfağı Tarifleri

🎯 **Ödeviniz:**  
GitHub’da bir repo oluşturup **bir dünya mutfağından yemek tarifi** ve **favori tatlınızın tarifini** ayrı dosyalarda yazacaksınız. Ardından, **repo’yu klonlayarak fotoğrafları ekleyip** GitHub’a yükleyeceksiniz.  

---

## 📌 Ödev Adımları  

### **1️⃣ GitHub’da Yeni Bir Repository (Repo) Oluşturun**  
1. **GitHub’a giriş yapın**: [GitHub](https://github.com/)  
2. Sağ üstte **“+”** simgesine tıklayın ve **“New repository”** seçeneğini seçin.  
3. **Repo Adı:** `dunya-mutfagi`  
4. **Açıklama (Description)** ekleyin.  
5. **Public (Herkese Açık) veya Private (Özel) seçeneğini belirleyin.**  
6. **"Add a README file"** seçeneğini işaretleyin.  
7. **"Create Repository"** butonuna tıklayın. 🎉  

---

### **2️⃣ Yeni Dosya Oluşturma ve İlk Tarifinizi Ekleyin**  
1. **Repo sayfanızda "Add file" → "Create new file" seçeneğine tıklayın.**  
2. **Dosya adı:** `dunya-mutfagindan-yemek.md`  
3. **İçeriği şu şekilde ekleyin:**  

   ```md
   # 🍛 [Seçtiğiniz Dünya Mutfağı Yemeği] Tarifi  

   ## 📌 Malzemeler:  
   - 🥩 X gram et  
   - 🧄 2 diş sarımsak  
   - 🧅 1 adet soğan  
   
   ## 👨‍🍳 Yapılışı:  
   1️⃣ Malzemeleri doğrayın ve karıştırın.  
   2️⃣ Tavada kısık ateşte pişirin.  
   ```
4. **“Commit new file” butonuna tıklayarak kaydedin.**  

---

### **3️⃣ Favori Tatlı Tarifinizi Ekleyin**  
1. **Tekrar "Add file" → "Create new file" seçeneğine tıklayın.**  
2. **Dosya adı:** `favori-tatlim.md`  
3. **İçeriği şu şekilde ekleyin:**  

   ```md
   # 🍰 Favori Tatlım Tarifi  

   ## 📌 Malzemeler:  
   - 🍯 1 su bardağı bal  
   - 🥛 2 su bardağı süt  
   - 🥚 2 yumurta  

   ## 👨‍🍳 Yapılışı:  
   1️⃣ Tüm malzemeleri karıştırın.  
   2️⃣ 180°C fırında 20 dakika pişirin.  
   ```
4. **“Commit new file” butonuna tıklayarak kaydedin.**  

---

### **4️⃣ Repo’yu Bilgisayarınıza Klonlayın ve Fotoğrafları Ekleyin**  
1. **Repo sayfanızda “Code” yeşil butonuna tıklayın ve **SSH**  linkini kopyalayın.**  
2. Terminal veya Git Bash açarak şu komutu çalıştırın:  

   ```bash
   git clone <repo-linkiniz>
   ```
   📌 **Örnek:**  
   ```bash
   git clone git@github.com:kullanici_adiniz/repo_adiniz.git
   ```  
3. Klonlanan klasöre girin:  
   ```bash
   cd dunya-mutfagi
   ```
4. **"images" adlı bir klasör oluşturun:**  
   ```bash
   mkdir images
   ```
5. **Bilgisayarınızdan yemek ve tatlı fotoğraflarını "images" klasörüne sürükleyin.**  
6. **Git’e ekleyin ve yükleyin:**  
   ```bash
   git add .
   git commit -m "Fotoğraflar eklendi"
   git push origin main
   ```

---

### **5️⃣ Ana README Dosyanızı Düzenleyin**  
1. **README.md dosyanızı açarak şu içeriği ekleyin:**  

   ```md
   # 🌍 Dünya Mutfağı Tarifleri  

   Bu repo, dünya mutfaklarından seçtiğim bir yemek ve en sevdiğim tatlı tarifini içermektedir.  

   ## 🍽️ Tariflerim  
   - [🍛 Dünya Mutfağından Yemek](./dunya-mutfagindan-yemek.md)  
   - [🍰 Favori Tatlım](./favori-tatlim.md)  

   ![Yemek](./images/yemek.jpg)  
   ![Tatlı](./images/tatli.jpg)  
   ```
2. **Değişiklikleri kaydedin ve GitHub’a yükleyin:**  
   ```bash
   git add README.md
   git commit -m "README güncellendi"
   git push origin main
   
