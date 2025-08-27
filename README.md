RESTful API - Products

Bu proje, basit bir RESTful API uygulamasıdır. Ürünlerle ilgili temel CRUD (Create, Read, Update, Delete) işlemlerini gerçekleştirmenin yanı sıra ürünleri listeleme ve sıralama işlevselliği de sağlar.

🔗 Endpoints

1. Ürünleri Listele
   GET /api/products
   Tüm ürünleri listeler.

2. Belirli Bir Ürünü Getir
   GET /api/products/{id}
   Belirtilen ID’ye sahip ürünü getirir.

3. Yeni Ürün Ekle
   POST /api/products
   Yeni bir ürün ekler.
   İstek gövdesinde JSON formatında ürün bilgileri bulunmalıdır.

4. Belirli Bir Ürünü Güncelle
   PUT /api/products/{id}
   Belirtilen ID’ye sahip ürünü günceller.
   İstek gövdesinde güncellenmiş ürün bilgileri bulunmalıdır.

5. Belirli Bir Ürünü Sil
   DELETE /api/products/{id}
   Belirtilen ID’ye sahip ürünü siler.

6. Ürünleri Listele ve Sırala
   GET /api/products/list?name={name}&sort={sort}
   Belirtilen isme göre filtreleme yapar ve isteğe bağlı olarak sıralama gerçekleştirir.

7. Belirli Bir Ürünü Parçalı Güncelle
   PATCH /api/products/{id}
   Belirtilen ID’ye sahip ürünü kısmi olarak günceller.
   İstek gövdesinde JSON Patch belgesi bulunmalıdır.

🚀 Kullanım

Projeyi yerel ortamda çalıştırmak için:

1. Projeyi klonlayın:
   git clone https://github.com/oguzhankoc55/RestfulApi.git

2. Proje dizinine gidin:
   cd RestfulApi

3. Projeyi çalıştırın:
   dotnet run

Uygulama çalıştığında yukarıdaki endpoint’ler üzerinden API’ye istek gönderebilirsiniz.

📦 Gereksinimler

- .NET Core SDK
- Bir HTTP istemci aracı (örn. cURL, Postman)

📑 Model

Ürün modeli aşağıdaki gibidir:

{
  "id": 1,
  "name": "Product 1",
  "price": 19.99
}
