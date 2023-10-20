# DesafioAPI
Java RESTful API criada para o desafio do Bootcamp Fullstack do santander.
## Diagrama de Classes

```mermaid

classDiagram
  class User {
    - name: String
    - account: Account
    - features: Feature[]
    - card: Card
    - news: News[]
  }

  class Account {
    - Number: String
    - Agency: String
    - Balance: Float
    - Limit: Float
  }

  class Feature {
    - icon: String
    - description: String
  }

  class Card {
    - Number: String
    - Limit: Float
  }

  class News {
    - icon: String
    - description: String
  }

  User "1" *-- "1" Account
  User "1" *-- "N" Feature
  User "1" *-- "1" Card
  User "1" *-- "N" News
```
