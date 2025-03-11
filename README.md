# OrangeHRM'e Yeni Dil Paketi Nasıl Eklenir?

OrangeHRM, farklı diller için çeviriler sağlamak amacıyla yeni dil paketleri eklemenize olanak tanır. OrangeHRM'e yeni bir dil paketi eklemek için aşağıdaki adımları izleyin.

---

## Adım 1: Dil Paketi Sayfasına Erişim
1. OrangeHRM hesabınıza yönetici ayrıcalıklarıyla giriş yapın.
2. Üst navigasyon menüsünde yer alan "Admin" sekmesine tıklayın.
3. "Configuration" seçeneğini seçin ve açılan menüden "Language Packages" (Dil Paketleri) seçeneğine tıklayın.
4. Bu adımları takip ederek OrangeHRM'de Dil Paketleri bölümüne erişebilirsiniz.

---

## Adım 2: Çeviri Yapılacak Dili Seçme
1. Dil Paketleri sayfasında, mevcut dillerin bir listesini göreceksiniz.
2. Çeviri yapmak istediğiniz dili bulun. Örneğin, Fransızca'yı seçebilirsiniz.
3. İlgili dilin yanındaki "Translate" (Çevir) butonuna tıklayın.

**Not:** Eğer çeviri yapmak istediğiniz dil listede yoksa, sayfanın üst kısmındaki "Add" (Ekle) butonuna tıklayın. Açılan pencereden yeni dil paketini seçin ve "Save" (Kaydet) butonuna tıklayarak dili ekleyin. Ardından, ilgili dilin "Translate" (Çevir) butonuna tıklayarak çeviri işlemine başlayın.

---

## Adım 3: Metinleri Çevirme
1. Çeviri yapmak istediğiniz dili seçtikten sonra, çeviri sayfasına yönlendirileceksiniz.
2. Gerekirse, üst kısımdaki filtreleri kullanarak çeviri seçeneklerini daraltabilirsiniz. Modül, kaynak metin ve çevrilmiş metin gibi filtreler kullanılabilir.
3. Bir kelime veya ifadeyi çevirmek için, ilgili metin kutusuna çeviriyi girin.

**Önemli!**
- Uygulamanın düzgün çalışması için `{ }` parantezleri içinde yer alan anahtar kelimeleri çevirmeyin.
- Çoğul ifadelerde yalnızca ana mesajı çevirin ve `count`, `plural`, `one`, `other` gibi anahtar kelimeleri değiştirmeyin.

**Örnek:**
Fransızca çeviri yapıyorsanız:

```plaintext
{count,plural, =0{No Records Found} one{(1) Record Found} other{ (#) Records Found}}

```Çeviri şu şekilde olmalıdır:
{count,plural, =0{Aucun enregistrement trouvé} one{(1) Enregistrement trouvé} other{ (#) Enregistrements trouvés}}

## Adım 4: Yeni Dili Uygulama
Yeni dili OrangeHRM örneğinize uygulamak için, Admin modülündeki "Configuration" (Yapılandırma) menüsüne gidin ve "Localization" (Yerelleştirme) seçeneğini seçin. Ardından, dil seçim alanına tıklayın ve yeni çevirdiğiniz dil paketini listede göreceksiniz. Dili seçin ve "Save" (Kaydet) butonuna tıklayın. Bu, yeni dili OrangeHRM örneğinize uygulayacaktır.
