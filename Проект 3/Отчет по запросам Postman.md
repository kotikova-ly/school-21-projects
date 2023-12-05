# Activities
## 1.  GET api/v1/Activities

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Activities

2. Ожидаемый результат - получение списка активностей

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0  
Accept: */*  
Cache-Control: no-cache  
Postman-Token: 66232927-211f-410a-8632-948a9bfe3f64  
Host: fakerestapi.azurewebsites.net  
Accept-Encoding: gzip, deflate, br  
Connection: keep-alive
```

4. Тело запроса  -

5. Заголовки ответа 
```
Content-Type: application/json; charset=utf-8; v=1.0  
Date: Wed, 20 Sep 2023 08:17:54 GMT  
Server: Kestrel  
Transfer-Encoding: chunked  
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id": 1,
  "title": "Activity 1",
  "dueDate": "2023-09-06T12:08:04.7927737+00:00",
  "completed": false
},
{
  "id": 2,
  "title": "Activity 2",
  "dueDate": "2023-09-06T13:08:04.7927761+00:00",
  "completed": true
},
```

## 2. POST ​/api​/v1​/Activities_val_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Activities{{activity_id}}

2. Ожидаемый результат - публикация активности

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 2f2a2045-ce59-4c04-8904-3e3bbf541d94
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-09-06T11:53:32.521Z",
  "completed": true
}
  ```

5. заголовки  ответа 
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 11:03:00 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id": 5,
  "title": "string",
  "dueDate": "2023-09-2111:03:32.521Z",
  "completed": true
}
```

## 3. POST ​/api​/v1​/Activities{{activity_id}} (-5)

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Activities{{activity_id}}

2. Ожидаемый результат - ошибка публикации активности

3. Заголовки запроса 
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 95e055d7-daec-4656-8c7c-50a2f14bdec2
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id":-5 ,
  "title": "string",
  "dueDate": Thu, 21 Sep 2023 11:53:30.874Z",
  "completed": true
}
```

5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 11:53:30 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":-5,
  "title":"string",
  "dueDate":"2023-09-21T07:32:04.317Z",
  "completed":true
}
```

## 4. POST ​/api​/v1​/Activities{{activity_id}} (10000000000)

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Activities{{activity_id}}
2. Ожидаемый результат - ошибка публикации активности
3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: c2dd9ece-e9c2-4d9e-9bef-46bbe4c76c30
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": 1000000000,
  "title": "string",
  "dueDate": "2023-09-21T07:32:04.317Z",
  "completed": true
}
```

5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 12:41:41 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":1000000000,
  "title":"string",
  "dueDate":"2023-09-21T07:32:04.317Z",
  "completed":true
}
```

## 5. Delet ​/api​/v1​/Activities 

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Activities{{activity_id}}

2. Ожидаемый результат - удаление  активностей по  id (1)

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: c2dd9ece-e9c2-4d9e-9bef-46bbe4c76c30
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса -
5. Заголовки ответа
```
Content-Length: 0
Date: Thu, 21 Sep 2023 13:25:24 GMT
Server: Kestrel
api-supported-versions: 1.0
```

6. Тело ответа -

## 6.  GET ​/api​/v1​/Activities{{activity_id}} (5)

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Activities{{activity_id}}

2. Ожидаемый результат - получение активности из списка

3. Заголовки запроса 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 52ca3627-5aa6-4e47-b4b5-ed503ae99d0b
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": 5,
  "title": "Activity 5",
  "dueDate": "2023-09-21T18:36:06.391161+00:00",
  "completed": false
}
```

5. Заголовки ответа 
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 13:36:05 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа
```
{
  "id":5,
  "title":"Activity 5",
  "dueDate":"2023-09-21T18:36:06.391161+00:00",
  "completed":false
}
```

## 7.  GET ​/api​/v1​/Activities​/{inv_neg_id} (-5)

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Activities{{activity_id}}

2. Ожидаемый результат - ошибка получения активности из списка

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: cd7f4fbd-c127-4608-8a49-6c182d7ece56
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": -5,
  "title": "Activity 5",
  "dueDate": "2023-09-21T18:36:06.391161+00:00",
  "completed": false
}
```
5. Заголовки ответа
```
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 13:39:03 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа
```
{
  "type":"https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title":"Not Found",
  "status":404,"traceId":"00-f89f8dd8781bff499c3031d4e6b388b6-d6c6c7ba92f5764b-00"
}
```

## 8.  GET ​/api​/v1​/Activities​/{inv_pos_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Activities{{activity_id}}

2. Ожидаемый результат - ошибка получения активности из списка

3. Заголовки запроса 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: c8cedf2b-20ab-4859-822f-a0bf727442b6
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса -

5. Заголовки ответа
```
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 13:45:44 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа
```
{
  "type":"https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title":"Not Found",
  "status":404,"traceId":"00-3d1226c683060b46b015a58807eae88d-1d6f94ab8b5ab346-00"
}
```

## 9.  PUT ​/api/v1/Activities/{val_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Activities{{activity_id}}

2. Ожидаемый результат - внесение изменения в активность 
3. Заголовки запроса 
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 89ca46dd-db9c-40fb-8339-06d4511611ed
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": 5,
  "title": "string",
  "dueDate": "2023-09-21T08:28:24.633Z",
  "completed": true
}
```

5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 13:58:48 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":5,
  "title":"string",
  "dueDate":"2023-09-21T08:28:24.633Z",
  "completed":true
}
```

## 10.  PUT api/v1/Activities/{inv_neg_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Activities{{activity_id}}

2. Ожидаемый результат - ошибка внесения изменения в активность 

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 61e79500-8292-49e5-9ba1-693545361085
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса
```
{
  "id": -5,
  "title": "string",
  "dueDate": "2023-09-21T08:28:24.633Z",
  "completed": true
}
```

5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 14:03:47 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа
``` 
{
  "id":-5,"title":"string",
  "dueDate":"2023-09-21T08:28:24.633Z",
  "completed":true}
```

## 11.  PUT api/v1/Activities/{inv_pos_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Activities{{activity_id}}

2. Ожидаемый результат - ошибка внесения изменения в активность

3. Заголовки запроса 
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 1e2037dc-b801-4abc-af57-37f517da9256
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": 1000000000,
  "title": "string",
  "dueDate": "2023-09-21T08:28:24.633Z",
  "completed": true
}
```

5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 21 Sep 2023 14:06:02 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа
``` 
{
  "id":1000000000,
  "title":"string",
  "dueDate":"2023-09-21T08:28:24.633Z",
  "completed":true
}
```

# Authors

## 1. POST /api​/v1​/Authors_pos_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors/{{activity_id}}

2. Ожидаемый результат - добавление нового автора

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 362359bd-b433-4047-bb33-9bec34c68b0d
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса
```
{
  "id": 5,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```

5. Заголовки ответа 
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 05:16:39 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа
```
{
  "id":5,
  "idBook":0,
  "firstName":"string",
  "lastName":"string"
}
```

## 2. POST /api​/v1​/Authors_inv_neg_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors/{{activity_id}}

2. Ожидаемый результат - ошибка добавления нового автора
3. Заголовки запроса 
 
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 362359bd-b433-4047-bb33-9bec34c68b0d
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": -5,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```

5. Заголовки ответа
``` 
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 05:16:39 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа
```
{
  "id":-5,
  "idBook":0,
  "firstName":"string",
  "lastName":"string"
}
```

## 3. POST /api​/v1​/Authors_inv_pos_id

1.  Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors/{{activity_id}}

2. Ожидаемый результат - ошибка добавления нового автора

3. Заголовки запроса
```
Content-Type: application/json
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 6e0fad64-0072-479c-a46b-fb12ecc9eff3
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса
```
{
  "id": 1000000000,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```

5. Заголовки ответа
``` 
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 05:57:50 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа
```
{
  "id":1000000000,
  "idBook":0,
  "firstName":"string",
  "lastName":"string"
}
```

## 4.  GET  /api​/v1​/Authors_pos_id

1.  Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors/{{activity_id}}

2. Ожидаемый результат - получение информации об авторе

3. Заголовки запроса

``` 
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: a74173b0-c05b-45ad-98bf-c036aec4a269
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": 5,
  "idBook": 2,
  "firstName": "First Name 5",
  "lastName": "Last Name 5"
}
```

5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 06:07:42 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа
``` 
{
  "id":5,
  "idBook":2,
  "firstName":"First Name 5",
  "lastName":"Last Name 5"
}
```

## 5.  GET /api/v1/Authors/{inv_neg_idAuthors}

1.  Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors/{{activity_id}}

2. Ожидаемый результат - ошибка получения информации об авторе

3. Заголовки запроса 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b72ecfeb-b570-44ac-8a8b-6b400df6ad6a
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-1c8804ec6fe30241ac0a01247b9e7e4a-036f645003490b4a-00"
}
```

5. Заголовки ответа
```
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 06:10:48 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "type":"https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title":"Not Found",
  "status":404,
  "traceId":"00-1c8804ec6fe30241ac0a01247b9e7e4a-036f645003490b4a-00"
}
```

## 6. GET  /api/v1/Authors/{inv_pos_idAuthors}
1.  Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors/{{activity_id}}

2. Ожидаемый результат - ошибка получения информации об авторе

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 81eee9cd-a413-4dff-8117-6087140ec660
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-f3023f7899f7f24b8ac3d22cbbb8ea72-0b741ba4601aab4d-00"
}
```

5. Заголовки ответа
```
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 06:14:24 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа
```
{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.4",
"title":"Not Found",
"status":404,
"traceId":"00-63ac24e3724c9e4fa14bd455bb040d47-ea7315b8435aea43-00"
}
```

## 7.  PUT  api/v1/Authors/{{valid_id}}

1.  Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors/{{activity_id}}

2. Ожидаемый результат - внесение изменений в информацию об авторе
3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 62ea8b4f-874d-4057-b6ab-36415a664499
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": 5,
  "idBook": 0,
  "firstName": null,
  "lastName": null
}
```

5. Заголовки ответа 
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 06:21:16 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа  
```
{
  "id":5,
  "idBook":0,
  "firstName":null,
  "lastName":null
}
```

## 8.  PUT  /api/v1/Authors/{inv_neg_id}

1.  Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors/{{invalid_negative_id}}

2. Ожидаемый результат - ошибка внесения изменений в информацию об авторе

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 99f0725e-d659-40aa-9be4-9e7dfb99f443
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса
```
{
  "id": -5,
  "idBook": 0,
  "firstName": null,
  "lastName": null
}
```

5. Заголовки ответа
``` 
CContent-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 06:24:53 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":-5,
  "idBook":0,
  "firstName":null,
  "lastName":null
}
```

## 9.  PUT  /api/v1/Authors/{{invalid_positive_id}}

1.  Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors/{{invalid_positive_id}}

2. Ожидаемый результат - ошибка внесения изменений в информацию об авторе

3. Заголовки запроса 

```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b5a0b592-d6b1-4081-804f-3232f587a238
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": 1000000000,
  "idBook": 0,
  "firstName": null,
  "lastName": null
}
```

5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 06:29:38 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":1000000000,
  "idBook":0,
  "firstName":null,
  "lastName":null
}
```

## 10. GET  /api/v1/Authors

1.  Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors

2. Ожидаемый результат - полчуние списка авторов

3. Заголовки запроса

```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 42c7db33-bcc6-4af0-a305-626fbe09879c
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 

```
{
  "id": 1,
  "idBook": 1,
  "firstName": "First Name 1",
  "lastName": "Last Name 1"
},
{
  "id": 2,
  "idBook": 1,
  "firstName": "First Name 2",
  "lastName": "Last Name 2"
},
{
  "id": 3,
  "idBook": 1,
  "firstName": "First Name 3",
  "lastName": "Last Name 3"
},
   
```

5. Заголовки ответа 

```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 06:42:31 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{"id":1,
"idBook":1,
"firstName":"First Name 1",
"lastName":"Last Name 1"
},
{
  "id":2,
  "idBook":1,
  "firstName":"First Name 2",
  "lastName":"Last Name 2"
},
{
  "id":3,
  "idBook":1,
  "firstName":"First Name 3",
  "lastName":"Last Name 3"
},
```

## 11. GET /api/v1/Authors/{val_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors/{{valid_id}}

2. Ожидаемый результат - получение информации об авторе из списка

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 4f854e89-31e9-41d3-9b61-311f3c38f016
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
4. Тело запроса 
```
{
  "id": 5,
  "idBook": 2,
  "firstName": "First Name 5",
  "lastName": "Last Name 5"
}
```

5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 06:50:49 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа
``` 
{
  "id":5,
  "idBook":2,
  "firstName":"First Name 5",
  "lastName":"Last Name 5"
}
```
  
## 12. GET   /api/v1/Authors/{inv_neg_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors/{{invalid_negative_id}}

2. Ожидаемый результат - ошибка получения информации об авторе из списка

3. Заголовки запроса
```
UUser-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 87430203-dd69-41a9-a776-d2611d0b36d2
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-d2a411499043ca439156ca5f60b0c691-0e5b44af74f92440-00"
}
```

5. Заголовки ответа 
```
CContent-Type: application/problem+json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 06:57:43 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "type":"https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title":"Not Found",
  "status":404,
  "traceId":"00-9ce7376f8dcf0e45ad2acce1e4581c23-738c09f794ae634d-00"
}
```

## 13. GET  /api/v1/Authors/{{invalid_positive_id}}

1. Полный URL запроса - 1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors/{{invalid_negative_id}}

2. Ожидаемый результат - ошибка получения информации об авторе из списка

3. Заголовки запроса 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 45f633f7-2481-47af-8e86-2181bcd1cc8f
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-d2a411499043ca439156ca5f60b0c691-0e5b44af74f92440-00"
}
```

5. Заголовки ответа

``` 
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 07:01:41 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "type":"https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title":"Not Found",
  "status":404,
  "traceId":"00-ed0d27622d1cfb41bbd10bf10b8cc01e-3cc6449712531e4f-00"
}
```

## 14. DELET /api/v1/Authors/{val_id}

1. Полный URL запроса - 1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Authors/{{invalid_negative_id}}

2. Ожидаемый результат - удаление автора

3. Заголовки запроса

```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 60f4ba5c-560a-45e7-b8f9-901dd05c1802
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса -

5. Заголовки ответа
```
Content-Length: 0
Date: Fri, 22 Sep 2023 07:04:43 GMT
Server: Kestrel
api-supported-versions: 1.0
```

6. Тело ответа -

# Books

## 1. GET ​/api​/v1​/Books

1. Полный URL запроса  - https://fakerestapi.azurewebsites.net/api/v1/Books

2. Ожидаемый результат - получение списка книг

3. Заголовки запроса 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 10741a64-3558-493f-9877-380bf7c8c7c0
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса
```
{
  "id": 1,
  "title": "Book 1",
  "description": "Erat stet stet facilisis dolor dolore lorem voluptua eu consetetur laoreet eum. Sed vero sanctus eos hendrerit velit sanctus lorem duis diam. Diam lorem iusto dolore volutpat invidunt iriure tincidunt gubergren nonumy sanctus clita. Sea amet dolor aliquip vero facilisi amet at gubergren nonumy sadipscing gubergren sea vero stet tation eirmod. Molestie doming aliquam ipsum accusam diam dolores tempor aliquyam ut lorem voluptua praesent.\n",
  "pageCount": 100,
  "excerpt": "Sed ut duo clita et sed ea gubergren dolore sed at justo tempor diam feugiat ipsum. Sed sit minim ut et commodo gubergren sadipscing. Nulla diam justo nihil diam ad. Kasd dolore eirmod elitr justo consequat eirmod diam dolore ipsum duo velit sed euismod. Kasd erat praesent ut suscipit sanctus option lorem vel ex sed dolore sadipscing diam dolores at.\nAmet no aliquyam clita tation iusto. Sit takimata praesent ut gubergren et vulputate. Nonumy esse diam et. \n",
  "publishDate": "2023-09-21T07:09:14.2230423+00:00"
},
```

5. Заголовки ответа 
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 07:09:13 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":1,
  "title":"Book 1",
  "description":"Erat stet stet facilisis dolor dolore lorem voluptua eu consetetur laoreet eum. Sed vero sanctus eos hendrerit velit sanctus lorem duis diam. Diam lorem iusto dolore volutpat invidunt iriure tincidunt gubergren nonumy sanctus clita. Sea amet dolor aliquip vero facilisi amet at gubergren nonumy sadipscing gubergren sea vero stet tation eirmod. \n",
  "pageCount":100,
  "excerpt":"Sed ut duo clita et sed ea gubergren dolore sed at justo tempor diam feugiat ipsum. Sed sit minim ut et commodo gubergren sadipscing. Nulla diam justo nihil diam ad. Kasd dolore eirmod elitr justo consequat eirmod diam dolore ipsum duo velit sed euismod. Kasd erat praesent ut suscipit sanctus option lorem vel ex sed dolore sadipscing diam dolores at.\n
  },
```
## 2.  POST  /api/v1/Books_val_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Books

2. Ожидаемый результат - публикация книги

3. Заголовки запроса 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 45f633f7-2481-47af-8e86-2181bcd1cc8f
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": 5,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-09-21T07:41:17.307Z"
}
```

5. Заголовки ответа
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 07:14:33 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":5,
  "title":"string",
  "description":"string",
  "pageCount":0,
  "excerpt":"string",
  "publishDate":"2023-09-21T07:41:17.307Z"
}
```

## 3. POST /api/v1/Books_inv_neg_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Books

2. Ожидаемый результат - ошибка публикации книги

3. Заголовки запроса 
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: d3ff5c4e-aed5-4651-96fd-7101df7473c8
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": -5,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-09-21T07:41:17.307Z"
}
```

5. Заголовки ответа 
``` 
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 07:23:05 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа  
```
{
  "id":-5,
  "title":"string",
  "description":"string",
  "pageCount":0,
  "excerpt":"string",
  "publishDate":"2023-09-21T07:41:17.307Z"
}
```

## 4.  POST  /api/v1/Books_inv_pos_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Books

2. Ожидаемый результат - ошибка публикации книги

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 8566b267-d10c-4e54-98d2-50c4f1afa0c1
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": 1000000000,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-09-21T07:41:17.307Z"
}
```

5. Заголовки ответа

``` 
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 07:23:05 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id": 1000000000,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-09-21T07:41:17.307Z"
}
```

## 5. GET /api/v1/Books/{val_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Books/5

2. Ожидаемый результат - получение информации о книге из списка

3. Заголовки запроса 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: f7bc1a7e-8462-41cc-a821-d828f95b1cc0
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": 5,
  "title": "Book 5",
  "description": "Vel ea sit erat duis. Commodo nonumy et augue ipsum nonumy ad vel takimata et sed elitr. Ut ea vel duo clita hendrerit dolor ipsum invidunt amet sanctus dolor sed at ut dolore facilisis stet amet. Aliquyam kasd dolor est et nonumy. Dolor no sanctus. Nulla vel sit eum takimata hendrerit ipsum et. Est takimata tempor wisi ut nulla duo nonumy invidunt dolore ea est et kasd. Eu lorem wisi nonumy sit sadipscing magna placerat dolor no. Iusto ut tempor nonummy et. Ullamcorper consetetur justo dolore vel lorem et et amet at aliquyam amet eirmod vulputate in erat esse dolor amet.\n",
}
```

5. Заголовки ответа 
``` 
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 07:23:05 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id": 5,
  "title": "Book 5",
  "description": "Vel ea sit erat duis. Commodo nonumy et augue ipsum nonumy ad vel takimata et sed elitr. Ut ea vel duo clita hendrerit dolor ipsum invidunt amet sanctus dolor sed at ut dolore facilisis stet amet. Aliquyam kasd dolor est et nonumy. Dolor no sanctus. Nulla vel sit eum takimata hendrerit ipsum et. Est takimata tempor wisi ut nulla duo nonumy invidunt dolore ea est et kasd. Eu lorem wisi nonumy sit sadipscing magna placerat dolor no. Iusto ut tempor nonummy et. Ullamcorper consetetur justo dolore vel lorem et et amet at aliquyam amet eirmod vulputate in erat esse dolor amet.\n",
}
``` 

## 6. GET /api/v1/Books/{inv_neg_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Books/-5

2. Ожидаемый результат - ошибка получения информации о книге из списка

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: cd79fda8-6d65-40a8-b456-0512afd3d003
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-526d5f1fd0a5d64b9e5d6f23e06a625e-56b16b3eb9d0bd47-00"
}
```

5. Заголовки ответа
``` 
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 07:31:48 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "type":"https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title":"Not Found",
  "status":404,
  "traceId":"00-526d5f1fd0a5d64b9e5d6f23e06a625e-56b16b3eb9d0bd47-00"
}
```

## 7.  GET /api/v1/Books/{inv_pos_id}
1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Books/1000000000

2. Ожидаемый результат - ошибка получения информации о книге из списка

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 0692039e-fee0-4cf2-9deb-1d9f86f9ee94
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-526d5f1fd0a5d64b9e5d6f23e06a625e-56b16b3eb9d0bd47-00"
}
```

5. Заголовки ответа 
```
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 07:31:48 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```
6. Тело ответа 
```
 {
  "type":"https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title":"Not Found",
  "status":404,
  "traceId":"00-2da039bed1aedf4bb9b81aebc67a36b5-76a2c382f264b049-00"
}
```

## 8. DELET /api/v1/Books/{val_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Books/5

2. Ожидаемый результат - удаление книги

3. Заголовки запроса 
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b255bde2-c2be-4014-8712-b2669f11bb9e
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  -

5. Заголовки ответа 
```
Content-Length: 0
Date: Fri, 22 Sep 2023 07:39:03 GMT
Server: Kestrel
api-supported-versions: 1.0
```

6. Тело ответа -

## 9. PUT /api/v1/Books/{val_id}

1. Полный URL запроса - PUT https://fakerestapi.azurewebsites.net/api/v1/Books/5

2. Ожидаемый результат - внесение изменений в информацию о книге

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: c095a7ec-51a1-4206-922f-4a2199c79f68
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса
```
{
  "id": 5,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-09-21T10:48:38.967Z"
}
```

5. Заголовки ответа
``` 
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 07:41:20 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":5,
  "title":"string",
  "description":"string",
  "pageCount":0,
  "excerpt":"string",
  "publishDate":"2023-09-21T10:48:38.967Z"
}
```

## 10. PUT /api/v1/Books/{inv_neg_id}

1. Полный URL запроса - PUT https://fakerestapi.azurewebsites.net/api/v1/Books/-5

2. Ожидаемый результат - ошибка внесения изменений в информацию о книге

3. Заголовки запроса  
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: c095a7ec-51a1-4206-922f-4a2199c79f68
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": -5,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-09-21T10:48:38.967Z"
}
```

5. Заголовки ответа 
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 07:41:20 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":-5,
  "title":"string",
  "description":"string",
  "pageCount":0,
  "excerpt":"string",
  "publishDate":"2023-09-21T10:48:38.967Z"
}
```

## 11.  PUT /api/v1/Books/{inv_pos_id}

1. Полный URL запроса - PUT https://fakerestapi.azurewebsites.net/api/v1/Books/1000000000

2. Ожидаемый результат - ошибка внесения изменений в информацию о книге

3. Заголовки запроса 
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: c095a7ec-51a1-4206-922f-4a2199c79f68
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса 
```
{
  "id": 1000000000,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-09-21T10:48:38.967Z"
}
```

5. Заголовки ответа -
``` 
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 07:46:12 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":1000000000,
  "title":"string",
  "description":"string",
  "pageCount":0,
  "excerpt":"string",
  "publishDate":"2023-09-21T10:48:38.967Z"
}
```

# CoverPhotos
## 1.  GET api/v1/CoverPhotos

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos

2. Ожидаемый результат - получение списка обложек

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 834df31a-23cb-410c-aff7-ed8bc68cabb5
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  - нет

5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 10:46:59 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
[
  {"id":1,
  "idBook":1,
  "url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
  },
  {"id":2,
  "idBook":2,
  "url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 2&w=250&h=350"
  },
  {"id":3,
  "idBook":3,
  "url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 3&w=250&h=350"
  },..
]
```  

## 2.  POST /api/v1/CoverPhotos_val_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos

2. Ожидаемый результат - Публикация обложки

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 33e2b030-f222-4557-bfcb-bc55b50f0462
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  
```
{
  "id": 5,
  "idBook": 0,
  "url": "string"
}
```

5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 10:50:53 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":5,
  "idBook":0,
  "url":"string"
}
```  

## 3.  POST /api/v1/CoverPhotos_inv_neg_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos

2. Ожидаемый результат - Ошибка публикации обложки

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b1726a82-4dba-45db-8309-b66be79f84c1
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  
```
{
  "id": -5,
  "idBook": 0,
  "url": "string"
}
```

5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 10:55:46 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":-5,
  "idBook":0,
  "url":"string"
}
```  

## 4.  POST /api/v1/CoverPhotos_inv_neg_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos

2. Ожидаемый результат - Ошибка публикации обложки

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: b1726a82-4dba-45db-8309-b66be79f84c1
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  
```
{
  "id": -5,
  "idBook": 0,
  "url": "string"
}
```

5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 10:55:46 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{"
 id":-5,
 "idBook":0,
 "url":"string"
}
```  

## 5.  GET /api/v1/CoverPhotos_val_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos

2. Ожидаемый результат - получение обложки из списка

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: fd5ae169-5d3a-451a-b600-75bf7afd8231
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса - Нет  


5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:00:12 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":5,
  "idBook":5,
  "url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 5&w=250&h=350"
}
```  

## 6.  GET /api/v1/CoverPhotos/{inv_neg_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/{{invalid_negative_id}}

2. Ожидаемый результат - ошибка получения обложки

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 13dd351e-a9c7-4d47-a96d-de9a0cecbc0a
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса - Нет  


5. Заголовки ответа  
```
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:05:32 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "type":"https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title":"Not Found",
  "status":404,
  "traceId":"00-43f4940b07ccd84394bb349f477a7520-9880a251d096d44a-00"
}
```  

## 7.  GET /api/v1/CoverPhotos/{inv_pos_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos

2. Ожидаемый результат - ошибка получения обложки

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 554cc2b7-4781-406b-a6e6-805b6cf5df18
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса - Нет  


5. Заголовки ответа  
```
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:08:18 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "type":"https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title":"Not Found",
  "status":404,
  "traceId":"00-6084dad764a8484b8dcbefe21ea8febc-a94afb42747b734d-00"
}
```  

## 8.  PUT /api/v1/CoverPhotos_val_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/{{valid_id}}

2. Ожидаемый результат - обновление обложки из списка

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: c5e3d3d9-b007-42fd-8fae-24f014bb996b
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  
```
{
  "id": 5,
  "idBook": 0,
  "url": "string"
}
```  

5. Заголовки ответа  
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: c5e3d3d9-b007-42fd-8fae-24f014bb996b
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```  

6. Тело ответа 
```
{
  "id":5,
  "idBook":0,
  "url":"string"
}
```  

## 9.  PUT /api/v1/CoverPhotos/{inv_neg_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/{{invalid_negative_id}}

2. Ожидаемый результат - ошибка обновления обложки

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: fe2b7b12-3234-4ab0-a257-6db88ff21bc6
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  
```
{
  "id": -5,
  "idBook": 0,
  "url": "string"
}
```  


5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:14:46 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```  

6. Тело ответа 
```
{
 "id":-5,
 "idBook":0,
 "url":"string"
}
```  

## 10.  PUT /api/v1/CoverPhotos/{inv_pos_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/{{invalid_positive_id}}

2. Ожидаемый результат - ошибка обновления обложки

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: feb79545-c0f4-4952-887b-f65e40e428f0
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  
```
{
  "id": 1000000000,
  "idBook": 0,
  "url": "string"
}
```  

5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:18:16 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```  

6. Тело ответа 
```
{
  "id":1000000000,
  "idBook":0,
  "url":"string"
}
```  

## 11.  DELETE /api/v1/CoverPhotos/{val_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/{{valid_id}}

2. Ожидаемый результат - Удаление обложки

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: dc3946ea-41e0-484e-89ed-5094fdb060c3
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса - Нет  



5. Заголовки ответа  
```
Content-Length: 0
Date: Fri, 22 Sep 2023 11:21:19 GMT
Server: Kestrel
api-supported-versions: 1.0
```  

6. Тело ответа - Нет 

## 12.  GET /api/v1/CoverPhotos/books/covers/{val_idBook}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/{{valid_id}}

2. Ожидаемый результат - получение обложки книги

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: e983104e-30dd-4831-969b-dd757fa0dc75
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса - Нет  


5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:25:21 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
[
  {
    "id":5,
    "idBook":5,
    "url":"https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 5&w=250&h=350"
  }
]
```  

## 13.  GET /api/v1/CoverPhotos/books/covers/{inv_neg_idBook}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/{{invalid_negative_id}}

2. Ожидаемый результат - ошибка получения обложки книги

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 04a89ea9-7cf0-473c-a42a-9a545676256a
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса - Нет  


5. Заголовки ответа  
```
ontent-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:27:02 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
  []
```  

## 14.  GET /api/v1/CoverPhotos/books/covers/{inv_pos_idBook}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/{{invalid_positive_id}}

2. Ожидаемый результат - ошибка получения обложки книги
```
Accept: */*
Cache-Control: no-cache
Postman-Token: 9829a6ed-d605-4aa0-91ff-cdda47cad301
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса - Нет  


5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:28:30 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
  []
```  

# Users

## 1.  GET api/v1/Users

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Users

2. Ожидаемый результат - получение списка пользователей

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 91603281-0939-46b0-942f-361cf41639d9
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  - нет

5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:31:12 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
[
  {
    "id":1,
    "userName":"User 1",
    "password":"Password1"
  },
  {
    "id":2,
    "userName":"User 2",
    "password":"Password2"
  },
  {
    "id":3,
    serName":"User 3",
    "password":"Password3"
  },..
]
```  

## 2.  POST /api/v1/Users_val_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Users

2. Ожидаемый результат - публикация данных пользователя

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: e45381b0-13fc-4f75-bbe1-a60daee095be
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  
```
{
  "id": 5,
  "userName": "string",
  "password": "string"
}
```

5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:37:38 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":5,
  "userName":"string",
  "password":"string"
}
```  

## 3.  POST /api/v1/Users_inv_neg_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Users

2. Ожидаемый результат - ошибка публикации данных пользователя

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: ec8f8789-76c1-4c83-a56a-6b28132e35d4
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  
```
{
  "id": -5,
  "userName": "string",
  "password": "string"
}
```

5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:39:03 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":-5,
  "userName":"string",
  "password":"string"
}
```  

## 4.  POST /api/v1/Users_inv_pos_id

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Users

2. Ожидаемый результат - ошибка публикации данных пользователя

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 61990cbb-e649-4892-9260-33b10d643167
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  
```
{
  "id":1000000000,
  "userName": "string",
  "password": "string"
}
```

5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:40:15 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":1000000000,
  "userName":"string",
  "password":"string"
}
```  

## 5.  PUT /api/v1/Users/{val_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Users/{{valid_id}}

2. Ожидаемый результат - Обновление данных пользователя

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 4899cdaf-dcc0-4801-9896-874d6ef100e8
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  
```
{
  "id": 5,
  "userName": "string",
  "password": "string"
}
```  

5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:44:13 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```  

6. Тело ответа 
```
{
  "id":5,
  "userName":"string",
  "password":"string"
}
```  

## 6.  PUT /api/v1/Users/{inv_neg_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Users/{{invalid_negative_id}}

2. Ожидаемый результат - ошибка обновления данных пользователя

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 2dae9fcf-7c20-4225-b3cf-065ec7c09675
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  
```
{
  "id": -5,
  "userName": "string",
  "password": "string"
}
```  

5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:45:40 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```  

6. Тело ответа 
```
{
  "id":-5,
  "userName":"string",
  "password":"string"
}
```  

## 7.  PUT /api/v1/Users/{inv_pos_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Users/{{invalid_positive_id}}

2. Ожидаемый результат - ошибка обновления данных пользователя

3. Заголовки запроса
```
Content-Type: application/json
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 6ef9f45a-8cd9-41bf-b1c1-dc12e88a4a23
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса  
```
{
  "id": 1000000000,
  "userName": "string",
  "password": "string"
}
```  

5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:47:10 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```  

6. Тело ответа 
```
{
  "id":1000000000,
  "userName":"string",
  "password":"string"
}
```  

## 8.  GET /api/v1/Users/{val_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Users/{{valid_id}}

2. Ожидаемый результат - получение данных пользователя из списка

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 80956d8c-ba78-4297-91be-2cb8ccaf1f41
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса - Нет  

5. Заголовки ответа  
```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:52:16 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "id":5,
  "userName":"User 5",
  "password":"Password5"
}
```  

## 9.  GET /api/v1/Users/{inv_neg_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Users/{{invalid_negative_id}}

2. Ожидаемый результат - ошибка получения данных пользователя 

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 224e1c8f-c048-49ba-83ef-7ecc0ea66a30
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса - Нет  


5. Заголовки ответа  
```
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:53:32 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "type":"https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title":"Not Found",
  "status":404,
  "traceId":"00-86345c091119f144940491e381ddcec0-a392d118a029384b-00"
}
```  

## 10.  GET /api/v1/Users/{inv_pos_id}
1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Users/{{invalid_positive_id}}

2. Ожидаемый результат - ошибка получения данных пользователя

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 7fb1c72f-69a3-4488-a995-f3f473f7a2ce
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса - Нет  


5. Заголовки ответа  
```
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Fri, 22 Sep 2023 11:54:43 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

6. Тело ответа 
```
{
  "type":"https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title":"Not Found",
  "status":404,
  "traceId":"00-e5f9e3e6a54fff4d8d26edd4134c573f-b3e24c5f6e63584d-00"
}
```  

## 11.  DELETE /api/v1/Users/{val_id}

1. Полный URL запроса - https://fakerestapi.azurewebsites.net/api/v1/Users/{{valid_id}}

2. Ожидаемый результат - Удаление данных пользователя

3. Заголовки запроса
```
User-Agent: PostmanRuntime/7.33.0
Accept: */*
Cache-Control: no-cache
Postman-Token: 9ae7148b-9cd9-4fa7-8af6-01e8b2e2aa0e
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```

4. Тело запроса - Нет  


5. Заголовки ответа  
```
Content-Length: 0
Date: Fri, 22 Sep 2023 11:56:26 GMT
Server: Kestrel
api-supported-versions: 1.0
```  

6. Тело ответа - Нет
