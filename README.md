<p align="center">
  <a href="https://github.com/berkerertan/Tobeto3A-NArchitecture.BootcampProject/graphs/contributors"><img src="https://img.shields.io/github/contributors/berkerertan/Tobeto3A-NArchitecture.BootcampProject.svg?style=for-the-badge"></a>
  <a href="https://github.com/berkerertan/Tobeto3A-NArchitecture.BootcampProject/network/members"><img src="https://img.shields.io/github/forks/berkerertan/Tobeto3A-NArchitecture.BootcampProject.svg?style=for-the-badge"></a>
  <a href="https://github.com/berkerertan/Tobeto3A-NArchitecture.BootcampProject/stargazers"><img src="https://img.shields.io/github/stars/berkerertan/Tobeto3A-NArchitecture.BootcampProject.svg?style=for-the-badge"></a>
  <a href="https://github.com/berkerertan/Tobeto3A-NArchitecture.BootcampProject/issues"><img src="https://img.shields.io/github/issues/berkerertan/Tobeto3A-NArchitecture.BootcampProject.svg?style=for-the-badge"></a>
  <a href="https://github.com/berkerertan/Tobeto3A-NArchitecture.BootcampProject/blob/master/LICENSE"><img src="https://img.shields.io/github/license/berkerertan/Tobeto3A-NArchitecture.BootcampProject.svg?style=for-the-badge"></a>
</p><br />

# CodeStorm Eğitim Platformu Backend API (.NET)

## Proje Açıklaması
Bu proje, CodeStorm Eğitim Platformu'nun backend API'sini sağlamaktadır. Clean Architecture prensiplerine dayanarak geliştirilmiş ve nArchitectureGen kullanılarak tasarlanmıştır. Proje, yüksek performanslı ve ölçeklenebilir bir yapı sunar.

## Özellikler

<table>
  <tr>
    <td>-Clean Architecture</td>
    <td>-CQRS (Command Query Responsibility Segregation)</td>
  </tr>
  <tr>
    <td>-Gelişmiş Repository Pattern</td>
    <td>-Rol Bazlı Erişim Kontrolü(Eğitmen, Öğrenci, Admin)</td>
  </tr>
  <tr>
    <td>-Dynamic Query</td>
    <td>-Pagination</td>
  </tr>
  <tr>
    <td>-OTP (One-Time Password)</td>
    <td>-JWT ile Kimlik Doğrulama</td>
  </tr>
  <tr>
    <td>-Serilog ile Loglama</td>
    <td>-Pdf Oluşturma (Sertifika)</td>
  </tr>
  <tr>
    <td>-Couldinary Medya Servisi</td>
    <td>-Global Exception Handling</td>
  </tr>
  <tr>
    <td>-MsSQL</td>
    <td>-Refresh Token ve Token Yenileme</td>
  </tr>
  <tr>
    <td>-Token İptali (Revoke Token)</td>
    <td>-Mail Service</td>
  </tr>
   <tr>
    <td>-Mediatr</td>
    <td></td>
  </tr>
</table>

## Mimari Yapı
Bu proje, Clean Architecture ve CQRS (Command Query Responsibility Segregation) prensiplerini benimsemektedir. Bu mimari yapı, projenin modüler, test edilebilir ve sürdürülebilir olmasını sağlar. CQRS pattern uygulamasında Mediatr kullanılmıştır.

### Dosya Yapısı

<p float="left">
  <img src="https://i.imgur.com/YyxiUPq.png" alt="Proje Görseli 1" width="500"/>
</p>

## 💻 nArchitectureGen Hakkında
<p align="center">
  <a href="https://github.com/kodlamaio-projects/nArchitecture"><img src="https://user-images.githubusercontent.com/53148314/194872467-827dc967-acee-4bca-88a2-59ed5695bebf.png" height="75"></a>
  <h3 align="center">nArchitectureGen
</h3>
  
Clean Architecture'dan ilham alınarak geliştirilen nArchitecture, ileri seviye geliştirme tekniklerini sergileyen bir monolit projedir. Proje, Clean Architecture, CQRS, Gelişmiş Repository, Dinamik Sorgulama, JWT, OTP, Google ve Microsoft Doğrulama, Rol Tabanlı Yönetim, Dağıtık Önbellekleme (Redis), Logging (Serilog), Elastic Search, Code Generator ve daha fazlasını içermektedir.

### Kullanım
#### API Dökümantasyonu
Projede kullanılan tüm API endpoint'leri ve detayları için Swagger UI kullanabilirsiniz.

## Özellikler
### Clean Architecture
Bu proje, modüler, test edilebilir ve sürdürülebilir bir yapı sağlamak için Clean Architecture prensiplerini uygular. Katmanlar arasındaki bağımlılıkları minimize eder ve iş mantığını UI, veritabanı veya diğer dış bağımlılıklardan bağımsız hale getirir.

### CQRS (Command Query Responsibility Segregation)
CQRS, komutların (veri değiştirme işlemleri) ve sorguların (veri okuma işlemleri) ayrılmasını sağlar. Bu, performans optimizasyonu ve daha iyi veri bütünlüğü sağlar.

## JWT ile Kimlik Doğrulama
<p float="left">
  <img src="https://i.imgur.com/fMvXXyO.png" alt="Proje Görseli 1" width="370"/>
</p>
JWT (JSON Web Token) kullanarak kullanıcıların kimliklerini doğrulama işlemleri yapılır. Bu, güvenli ve stateless bir kimlik doğrulama yöntemi sunar. Decode JWT Payload kısmı görseldeki gibidir.

## OTP (One-Time Password)
Kullanıcıların kimliklerini doğrulamak için tek seferlik şifreler kullanılarak ekstra bir güvenlik katmanı sağlıyoruz.

## Serilog ile Loglama
<p float="left">
  <img src="https://i.imgur.com/GSNMuIF.png" alt="Proje Görseli 1" width="240"/>
</p>
Serilog kullanarak, uygulamada oluşan loglar yapılandırılır ve kayıt edilir. Bu, hata ayıklama ve uygulama izleme açısından oldukça faydalıdır. Mevcut demoda log kayıtları txt dosyası olarak saklanır, MongoDb kullanımı için altyapı mevcuttur.

## Dynamic Query
Dinamik sorgulama yetenekleri, kullanıcıların veya uygulamanın ihtiyaçlarına göre esnek ve özelleştirilebilir sorgular oluşturmasına olanak tanır.

## Global Exception Handling
Global hata yönetimi, uygulamanın herhangi bir yerinde oluşabilecek hataları merkezi bir noktada yakalayarak yönetmeyi sağlar. Bu, daha tutarlı hata mesajları ve daha iyi bir kullanıcı deneyimi sunar.

## Refresh Token ve Token Yenileme
<p float="left">
  <img src="https://i.imgur.com/rgxDMz5.png" alt="Proje Görseli 1" width="650"/>
</p>
Refresh token kullanarak, kullanıcıların oturum sürelerini uzatıyoruz. Böylece kullanıcılar tekrar giriş yapmak zorunda kalmıyor. Kullanıcı çıkış yaptığında veya güvenlik ihlali durumunda, token iptal edilerek erişim engellenir. RefreshToken HttpOnly Cookie yapıda kullanıcı giriş yaptığında oluşturulur. HttpOnly türü bu cookie'nin sadece http istekleri beraberinde taşınmasına olanak sağlar.

## Token İptali (Revoke Token)
Token iptali, kullanıcıların oturumlarını manuel olarak sonlandırmalarını veya güvenlik ihlallerinde erişimi engellemeyi sağlar. Bu, uygulamanın güvenliğini artıran önemli bir özelliktir.

## PDF Oluşturma (Sertifika)
<p float="left">
  <img src="https://i.imgur.com/XVNCUgM.png" alt="Proje Görseli 1" width="300"/>
  <img src="https://i.imgur.com/uriLTyr.png" alt="Proje Görseli 2" width="200"/>
</p>
Projemizde, kullanıcıların eğitimlerini tamamladıklarında sertifika üretmek için iTextSharp kütüphanesini kullanıyoruz. Bu kütüphane, PDF dosyalarını dinamik olarak oluşturup düzenlememize olanak tanır. Kullanıcıların kurs tamamlama sertifikaları gibi belgeleri PDF formatında oluşturmasını sağlar. Bu, kullanıcıya somut bir başarı göstergesi sunar ve platformun profesyonelliğini artırır.

## Mail Service
<p float="left">
  <img src="https://i.imgur.com/YI98iYV.png" alt="Proje Görseli 1" width="370"/>
</p>
Kullanıcılara e-posta göndermek için MailKit kütüphanesini ve Gmail'in SMTP sunucusunu kullanıyoruz. Bu yapı, e-posta doğrulama, şifre sıfırlama gibi işlemleri gerçekleştirmek için güvenilir ve esnek bir çözüm sunar. Kullanıcılarla iletişim kurmanın ve çeşitli işlemler (şifre sıfırlama, hesap doğrulama, iki faktörlü kimlik doğrulama) için e-posta gönderilir. Bu, kullanıcı deneyimini ve güvenliğini artırır. Mail gövdeleri Html dosyası olarak saklanır, mail gönderilme durumunda isteğe uygun dosya içerisindeki link veya tek seferlik kod alanı doldurulup gönderiyoruz.

## Veritabanı Şeması ve Request-Response Body Örnekleri
<table>
  <!-- row 1 -->
  <tr>
    <td colspan="3" align="center">
      <img src="https://i.imgur.com/WFJIROU.png" alt="default-header" width="900"/><br>
      <code>Veritabanı Diagramı</code>
    </td>
  </tr>
  <!-- row 2 -->
  <tr>
    <td align="center">
      <img src="https://i.imgur.com/qIPlDzW.png" alt="cloud-db-logo" width="300"/><br>
      <code>Başarılı Login Durumunda Response</code>
    </td>
    <td align="center">
      <img src="https://i.imgur.com/0x5Ibhi.png" alt="cloud-db-logo" width="300"/><br>
      <code>Login Request</code>
    </td>
    <td align="center">
      <img src="https://i.imgur.com/V9acTLn.png" alt="gradient-markdown-logo" width="300"/><br>
      <code>Oluşturulan Sertifikalar</code>
    </td>
  </tr>
  <!-- row 3 -->
  <tr>
    <td align="center">
      <img src="https://i.imgur.com/LaE9tu3.png" alt="custom-logo" width="300"/><br>
      <code>Hata Durumunda Response</code>
    </td>
    <td align="center">
      <img src="https://i.imgur.com/NB66lcs.png" alt="skills-light" width="300"/><br>
      <code>Öğrenci Kayıt Şeması</code>
    </td>
    <td align="center">
      <img src="https://i.imgur.com/PT8pBDT.png" alt="gradient-markdown-logo" width="300"/><br>
      <code>Command Request</code>
    </td>
  </tr>
  <tr>
  <!-- row 4 -->
    <td align="center">
      <img src="https://i.imgur.com/ubNu8Gl.png" alt="readme-ai-header" width="300"/><br>
      <code>Eğitim Oluşturma Şeması</code>
    </td>
    <td align="center">
      <img src="https://i.imgur.com/D30SOJG.png" alt="black-logo" width="300"/><br>
      <code>Sertifika Oluşturma Şeması</code>
    </td>
    <td align="center">
      <img src="https://i.imgur.com/tyQXhD9.png" alt="gradient-markdown-logo" width="300"/><br>
      <code>Chapter Request</code>
    </td>
  </tr>
</table>

### Katkıda Bulunma Rehberi

Bu projeye katkıda bulunmak istiyorsanız, lütfen aşağıdaki adımları izleyin:

- Depoyu fork edin.
- Yeni bir dal (branch) oluşturun: git checkout -b my-new-feature
- Yaptığınız değişiklikleri commit edin: git commit -am 'Add some feature'
- Dalınıza (branch) push edin: git push origin my-new-feature
- Bir Pull Request oluşturun.

### İletişim
Bu proje hakkında herhangi bir sorunuz veya geri bildiriminiz varsa, lütfen buradan bizimle iletişime geçin.

## Teşekkürler
