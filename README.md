# Bekarevi - Ortak Ev Gider Yönetim Uygulaması

Bekarevi, ev arkadaşları, öğrenciler veya ortak yaşam alanlarını paylaşan herkes için geliştirilmiş modern bir gider takip ve yönetim uygulamasıdır. Bu uygulama sayesinde ev harcamaları şeffaf bir şekilde yönetilebilir, borç-alacak takibi kolayca yapılabilir.



---

## 🚀 Temel Özellikler

- **Ev Oluşturma ve Yönetme:** Kullanıcılar kendi "evlerini" oluşturarak yönetici (admin) olabilirler.
- **Davet Kodu Sistemi:** Ev yöneticileri, evlerine özel, benzersiz bir davet kodu ile arkadaşlarını davet edebilir.
- **Onay Mekanizması:** Bir eve katılma talepleri, ev yöneticisinin onayına sunulur. Yönetici, talepleri panel üzerinden onaylayabilir veya reddedebilir.
- **Kullanıcı Yönetimi:** Yöneticiler, mevcut ev üyelerini görüntüleyebilir ve evden çıkarabilir.
- **Rol Tabanlı Yetkilendirme:** Sistemde `admin` ve `member` (üye) olmak üzere iki farklı kullanıcı rolü bulunmaktadır.
- **Dinamik Arayüz:** Kullanıcının durumuna (bir eve sahip olup olmaması, başvurusunun beklemede olması vb.) göre farklı arayüzler gösterilir.

---

## 🛠️ Kullanılan Teknolojiler

- **Frontend:** [React](https://reactjs.org/)
- **Dil:** [TypeScript](https://www.typescriptlang.org/)
- **Build Aracı:** [Vite](https://vitejs.dev/)
- **Backend & Veritabanı:** [Firebase](https://firebase.google.com/)
  - **Authentication:** Kullanıcı girişi ve kaydı için.
  - **Firestore:** Veritabanı olarak (evler, kullanıcılar, harcamalar vb.).
- **Styling:** Özel CSS

---

## 💻 Projeyi Yerel Makinede Çalıştırma

Projeyi kendi bilgisayarınızda çalıştırmak için aşağıdaki adımları izleyin.

### Gereksinimler
- [Node.js](https://nodejs.org/en/) (v16 veya üstü)
- `npm` veya `yarn` paket yöneticisi

### Kurulum Adımları

1.  **Projeyi klonlayın:**
    ```bash
    git clone [https://github.com/Abdulhadialayoub/Bekarevi.git](https://github.com/Abdulhadialayoub/Bekarevi.git)
    ```

2.  **Proje dizinine gidin:**
    ```bash
    cd Bekarevi
    ```

3.  **Gerekli paketleri yükleyin:**
    ```bash
    npm install
    ```

4.  **Firebase Kurulumu:**
    - Firebase konsolunda yeni bir proje oluşturun.
    - Projenize bir **Web Uygulaması** ekleyin ve size verilen `firebaseConfig` bilgilerini kopyalayın.
    - Projenin ana dizininde **`.env.local`** adında bir dosya oluşturun.
    - Kopyaladığınız bilgileri aşağıdaki formatta bu dosyaya yapıştırın:
      ```env
      VITE_FIREBASE_API_KEY="AIzaSy..."
      VITE_FIREBASE_AUTH_DOMAIN="proje-adin.firebaseapp.com"
      VITE_FIREBASE_PROJECT_ID="proje-adin"
      VITE_FIREBASE_STORAGE_BUCKET="proje-adin.appspot.com"
      VITE_FIREBASE_MESSAGING_SENDER_ID="123456789"
      VITE_FIREBASE_APP_ID="1:123456789:web:abcdef123"
      ```
    - Firebase projenizde **Authentication** (E-posta/Şifre metodu) ve **Firestore Database** (Test modunda başlatabilirsiniz) servislerini aktif ettiğinizden emin olun.

5.  **Geliştirme sunucusunu başlatın:**
    ```bash
    npm run dev
    ```
    Uygulama artık `http://localhost:5173` (veya terminalde belirtilen port) adresinde çalışıyor olacaktır.

---

## 🤝 Katkıda Bulunma

Katkılarınız projeyi daha iyi hale getirecektir! Katkıda bulunmak isterseniz, lütfen bir `pull request` açın veya bir `issue` oluşturun.

1.  Projeyi fork'layın.
2.  Yeni bir branch oluşturun (`git checkout -b ozellik/yeni-ozellik`).
3.  Değişikliklerinizi commit'leyin (`git commit -m 'Yeni özellik eklendi'`).
4.  Branch'inizi push'layın (`git push origin ozellik/yeni-ozellik`).
5.  Bir Pull Request açın.

---

## 📄 Lisans

Bu proje, MIT Lisansı ile lisanslanmıştır. Daha fazla bilgi için `LICENSE` dosyasına bakınız.

---

**Abdulhadi Alayoub** - [GitHub](https://github.com/Abdulhadialayoub)
