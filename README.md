## Navbar
[Product Api Collection](#product-api-collection)
- [Get Products](###get-products)
- [Grab Single Product](###get-single-product)
- [Add New Product ](###add-new-product)
- [Update Existing Product](###update-existing-product)
- [Delete Existing Product](###delete-existing-product)

# Product Api Collection
You need to get the <strong>token</strong> from our <strong>service</strong> page to get access to Product Api Collection.

### Get Products
#### Using JavaScript
```js
var axios = require('axios');
var data = JSON.stringify({
  "token": "Fpyr4JvT0v1BTfOIAakVxdBoayGljzY4JgBQEIO1gBOakof4KI5jya7RZrjzDcTb8zAJfSoOu5aicjm28fq6d0yak3L4OD0HXYSS"
});

var config = {
  method: 'post',
  url: 'https://ohhmart.com/api/test/product/vendor/2',
  headers: { 
    'Content-Type': 'application/json'
  },
  data : data
};

axios(config)
.then(function (response) {
  console.log(JSON.stringify(response.data));
})
.catch(function (error) {
  console.log(error);
});
```

#### Using Dart
```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://ohhmart.com/api/test/product/vendor/2'));
request.body = '''{\r\n    "token": "Fpyr4JvT0v1BTfOIAakVxdBoayGljzY4JgBQEIO1gBOakof4KI5jya7RZrjzDcTb8zAJfSoOu5aicjm28fq6d0yak3L4OD0HXYSS"\r\n}''';
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

#### Json
```json
{
    "data": {
        "id": 2,
        "productName": "Updated Lorem Ipsum",
        "productMedia": [],
        "productDescription": "Update Lorem Ipsum Description",
        "productCurrency": "USD",
        "productPrice": "20",
        "compareAtPrice": "10",
        "productWeight": "0.2 kg",
        "productType": "pants",
        "productTags": [
            "pants",
            "red",
            "yellow",
            "green"
        ],
        "productCollection": "women clothes",
        "vendorId": "1",
        "created_at": "2021-05-05T20:33:20.000000Z",
        "updated_at": "2021-05-05T21:01:04.000000Z",
        "shippingDetails": []
    }
}
```


### Grab Single Product

#### Using JavaScript
```js
var axios = require('axios');
var data = JSON.stringify({
  "token": "Fpyr4JvT0v1BTfOIAakVxdBoayGljzY4JgBQEIO1gBOakof4KI5jya7RZrjzDcTb8zAJfSoOu5aicjm28fq6d0yak3L4OD0HXYSS"
});

var config = {
  method: 'post',
  url: 'https://ohhmart.com/api/test/product/vendor/2',
  headers: { 
    'Content-Type': 'application/json'
  },
  data : data
};

axios(config)
.then(function (response) {
  console.log(JSON.stringify(response.data));
})
.catch(function (error) {
  console.log(error);
});
```

#### Using Dart
```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://ohhmart.com/api/test/product/vendor/2'));
request.body = '''{\r\n    "token": "Fpyr4JvT0v1BTfOIAakVxdBoayGljzY4JgBQEIO1gBOakof4KI5jya7RZrjzDcTb8zAJfSoOu5aicjm28fq6d0yak3L4OD0HXYSS"\r\n}''';
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

#### Json
```json
{
    "data": {
        "id": 2,
        "productName": "Updated Lorem Ipsum",
        "productMedia": [],
        "productDescription": "Update Lorem Ipsum Description",
        "productCurrency": "USD",
        "productPrice": "20",
        "compareAtPrice": "10",
        "productWeight": "0.2 kg",
        "productType": "pants",
        "productTags": [
            "pants",
            "red",
            "yellow",
            "green"
        ],
        "productCollection": "women clothes",
        "vendorId": "1",
        "created_at": "2021-05-05T20:33:20.000000Z",
        "updated_at": "2021-05-05T21:01:04.000000Z",
        "shippingDetails": []
    }
}
```


### Add New Product 

#### Using JavaScript
```js
var axios = require('axios');
var data = JSON.stringify({
  "token": "Fpyr4JvT0v1BTfOIAakVxdBoayGljzY4JgBQEIO1gBOakof4KI5jya7RZrjzDcTb8zAJfSoOu5aicjm28fq6d0yak3L4OD0HXYSS",
  "productName": "Lorem Ipsum",
  "productDescription": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
  "productCurrency": "NPR",
  "productPrice": "2000",
  "compareAtPrice": "1000",
  "productQuantity": "200",
  "productTags": "clothes, men, summer",
  "productCollection": "men clothes",
  "productWeight": "0.5 kg",
  "productType": "clothes"
});

var config = {
  method: 'post',
  url: 'https://ohhmart.com/api/test/product/vendor',
  headers: { 
    'Content-Type': 'application/json'
  },
  data : data
};

axios(config)
.then(function (response) {
  console.log(JSON.stringify(response.data));
})
.catch(function (error) {
  console.log(error);
});
```

#### Using Dart
```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://ohhmart.com/api/test/product/vendor'));
request.body = '''{\r\n    "token": "Fpyr4JvT0v1BTfOIAakVxdBoayGljzY4JgBQEIO1gBOakof4KI5jya7RZrjzDcTb8zAJfSoOu5aicjm28fq6d0yak3L4OD0HXYSS",\r\n    "productName": "Lorem Ipsum",\r\n    "productDescription": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry\'s standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",\r\n    "productCurrency": "NPR",\r\n    "productPrice": "2000",\r\n    "compareAtPrice": "1000",\r\n    "productQuantity": "200",\r\n    "productTags": "clothes, men, summer",\r\n    "productCollection": "men clothes",\r\n    "productWeight": "0.5 kg",\r\n    "productType": "clothes"\r\n}''';
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

#### Json
```json
{
    "response": {
        "productName": "Lorem Ipsum",
        "productDescription": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
        "productCurrency": "NPR",
        "productPrice": "2000",
        "compareAtPrice": "1000",
        "productQuantity": "200",
        "productWeight": "0.5 kg",
        "productType": "clothes",
        "productTags": "clothes, men, summer",
        "productCollection": "men clothes",
        "vendorId": 1,
        "message": "Product is created"
    }
}
```

### Update Existing Product

#### Using JavaScript
```js
var axios = require('axios');
var data = JSON.stringify({
  "token": "Fpyr4JvT0v1BTfOIAakVxdBoayGljzY4JgBQEIO1gBOakof4KI5jya7RZrjzDcTb8zAJfSoOu5aicjm28fq6d0yak3L4OD0HXYSS",
  "productName": "Updated Lorem Ipsum",
  "productDescription": "Update Lorem Ipsum Description",
  "productCurrency": "USD",
  "productPrice": "20",
  "compareAtPrice": "10",
  "productQuantity": "1000",
  "productWeight": "0.2 kg",
  "productType": "pants",
  "productTags": [
    "pants",
    "red",
    "yellow",
    "green"
  ],
  "productCollection": "women clothes"
});

var config = {
  method: 'post',
  url: 'https://ohhmart.com/api/test/product/vendor/update/2',
  headers: { 
    'Content-Type': 'application/json'
  },
  data : data
};

axios(config)
.then(function (response) {
  console.log(JSON.stringify(response.data));
})
.catch(function (error) {
  console.log(error);
});
```

#### Using Dart
```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://ohhmart.com/api/test/product/vendor/update/2'));
request.body = '''{\r\n    "token": "Fpyr4JvT0v1BTfOIAakVxdBoayGljzY4JgBQEIO1gBOakof4KI5jya7RZrjzDcTb8zAJfSoOu5aicjm28fq6d0yak3L4OD0HXYSS",\r\n    "productName": "Updated Lorem Ipsum",\r\n    "productDescription": "Update Lorem Ipsum Description",\r\n    "productCurrency": "USD",\r\n    "productPrice": "20",\r\n    "compareAtPrice": "10",\r\n    "productQuantity": "1000",\r\n    "productWeight": "0.2 kg",\r\n    "productType": "pants",\r\n    "productTags": [\r\n        "pants", "red", "yellow", "green"\r\n    ],\r\n    "productCollection": "women clothes"\r\n}''';
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

#### Json
```json
{
    "response": {
        "id": 2,
        "productName": "Updated Lorem Ipsum",
        "productDescription": "Update Lorem Ipsum Description",
        "productCurrency": "USD",
        "productPrice": "20",
        "compareAtPrice": "10",
        "productQuantity": "1000",
        "productWeight": "0.2 kg",
        "productType": "pants",
        "productTags": [
            "pants",
            "red",
            "yellow",
            "green"
        ],
        "productCollection": "women clothes",
        "message": "Product is updated successfully"
    }
}
```


### Delete Existing Product

#### Using JavaScript
```js
var axios = require('axios');
var data = JSON.stringify({
  "token": "Fpyr4JvT0v1BTfOIAakVxdBoayGljzY4JgBQEIO1gBOakof4KI5jya7RZrjzDcTb8zAJfSoOu5aicjm28fq6d0yak3L4OD0HXYSS"
});

var config = {
  method: 'post',
  url: 'https://ohhmart.com/api/test/product/vendor/delete/1',
  headers: { 
    'Content-Type': 'application/json'
  },
  data : data
};

axios(config)
.then(function (response) {
  console.log(JSON.stringify(response.data));
})
.catch(function (error) {
  console.log(error);
});
```

#### Using Dart
```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://ohhmart.com/api/test/product/vendor/delete/1'));
request.body = '''{\r\n    "token": "Fpyr4JvT0v1BTfOIAakVxdBoayGljzY4JgBQEIO1gBOakof4KI5jya7RZrjzDcTb8zAJfSoOu5aicjm28fq6d0yak3L4OD0HXYSS"\r\n}''';
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

#### Json
```json
{
    "response": "Product is deleted"
}
```
