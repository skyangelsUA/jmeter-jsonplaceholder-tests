Результати тестування JSONPlaceholder за допомогою JMeter

Дата тестування - 01.02.2025
Версія Jmeter 5.6.2
API JSONPlaceholder (https://jsonplaceholder.typicode.com)

Thread Group - 3 користувачf, 3 ітерації, 10 секунд на ітерацію.
Запити - GET, POST, PUT, PATCH, DELETE.

1.GET /posts/1
   Статус код 200
   Response Body
     {
      "userId": 1,
      "id": 1,
      "title": "sunt aut facere repellat provident occaecati excepturi optio reprehenderit",
      "body": "quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto"
     }
    Середній час запиту - 69 ms
    
2.POST /posts
  Статус код 201
  Response Body - 
    {
      "id": 101
    }
  Середній час запиту - 194 ms 

3.PUT /posts/1
  Статус код 200
  Response Body
    {
      "id": 1,
      "title": "foo",
      "body": "bar",
      "userId": 1
    }
  Середній час запиту - 187 ms

4.PATCH /posts/1
  Статус код 200
   Response Body
     {
      "userId": 1,
      "id": 1,
      "title": "sunt aut facere repellat provident occaecati excepturi optio reprehenderit",
      "body": "quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto"
    }
  Середній час запиту - 134 ms

5.DELETE /posts/1
  Статус код 200
  Response Body
    Відсутній
  Середній час запиту - 136 ms
  
