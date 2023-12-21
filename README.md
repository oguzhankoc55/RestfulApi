# RESTful API - Products

Bu proje, basit bir RESTful API'yi uygular ve ürünlerle ilgili temel CRUD (Create, Read, Update, Delete) işlemlerini gerçekleştirir. Ayrıca, ürünleri listeleyip sıralama işlevselliği de içerir.

## Endpoints

### 1. Ürünleri Listele [GET /api/products]

Tüm ürünleri listeler.

### 2. Belirli Bir Ürünü Getir [GET /api/products/{id}]

Belirtilen ID'ye sahip bir ürünü getirir.

### 3. Yeni Ürün Ekle [POST /api/products]

Yeni bir ürün ekler. İstek gövdesinde JSON formatında ürün bilgilerini içermelidir.

### 4. Belirli Bir Ürünü Güncelle [PUT /api/products/{id}]

Belirtilen ID'ye sahip bir ürünü günceller. İstek gövdesinde güncellenmiş ürün bilgilerini içermelidir.

### 5. Belirli Bir Ürünü Sil [DELETE /api/products/{id}]

Belirtilen ID'ye sahip bir ürünü siler.

### 6. Ürünleri Listele ve Sırala [GET /api/products/list?name={name}&sort={sort}]

Belirtilen isme göre filtreleme yapar ve isteğe bağlı olarak sıralama yapar.

### 7. Belirli Bir Ürünü Parçalı Güncelle [PATCH /api/products/{id}]

Belirtilen ID'ye sahip bir ürünü parçalı olarak günceller. İstek gövdesinde JSON Patch belgesini içermelidir.

## Model

Ürün modeli aşağıdaki gibidir:

```json
{
  "id": 1,
  "name": "Product 1",
  "price": 19.99
}
Kullanım
Projeyi yerel olarak çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

Projeyi klonlayın: git clone https://github.com/kullaniciadi/RestfulApi.git
Projeye gidin: cd RestfulApi
Projeyi çalıştırın: dotnet run
Proje çalıştığında, yukarıda belirtilen endpoint'leri kullanarak API'ye istekler yapabilirsiniz.

Gereksinimler
.NET Core SDK
Bir HTTP istemcisine sahip bir araç (örneğin, cURL veya Postman)