### CREATE DATABASE IF NOT EXISTS db01;
- Amaç: db01 adlı bir veritabanı oluşturur. Eğer db01 veritabanı zaten mevcutsa, hata vermeden işlemi atlar.
- Kullanım: Yeni bir veritabanı oluşturmak istediğinde, ancak aynı isimde bir veritabanı zaten var olup olmadığını kontrol etmek için kullanılır.
###  ALTER DATABASE db01 READ ONLY = 1;
- Amaç: db01 veritabanını salt okunur (read-only) moda geçirmeye çalışır. Ancak, MySQL'de ALTER DATABASE komutuyla doğrudan veritabanını salt okunur yapma desteği bulunmaz; bu komut çalışmaz.
- Not: MySQL'de salt okunur durumu daha çok tablo seviyesinde veya kullanıcı izinleriyle ayarlanabilir.
### USE db01;
- Amaç: db01 veritabanını aktif olarak kullanmak için seçer. Bu komut, sonraki SQL komutlarının hangi veritabanı üzerinde çalışacağını belirler.
- Kullanım: Bir veritabanı seçmek için kullanılır. Örneğin, sorgular ve tablolar üzerinde çalışmak için önce bu komutla veritabanını seçmelisin.
### DROP DATABASE db01;
- Amaç: db01 adlı veritabanını ve içindeki tüm verileri kalıcı olarak siler.
- Kullanım: Bir veritabanını ve onunla ilişkili tüm verileri geri dönüşü olmaksızın silmek istediğinde kullanılır. Dikkatli kullanılması gereken bir komuttur.
### ALTER DATABASE db01 READ ONLY = 0;
- Amaç: db01 veritabanını yazma ve okuma izinleriyle normal moda geri döndürmeyi amaçlar. Ancak, yukarıda bahsedildiği gibi, bu komut MySQL'de geçerli değildir.
- Not: MySQL'de salt okunur mod genellikle veritabanı seviyesinde değil, tablo seviyesinde veya kullanıcı izinleriyle kontrol edilir.
