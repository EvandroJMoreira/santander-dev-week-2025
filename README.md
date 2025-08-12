# Santander Dev Week 2025 - Dio
Java RESTful API criada para Santander Dev - Dio

## Diagrama de Classes
```mermaid
classDiagram
    class Usuario {
        string name
    }

    class Conta {
        string number
        string agency
        float balance
        float limit
    }

    class Feature {
        string icon
        string description
    }

    class Cartao {
        string number
        float limit
    }

    class Noticia {
        string icon
        string description
    }

    Usuario --> Conta : account
    Usuario --> "1..*" Feature : features
    Usuario --> Cartao : card
    Usuario --> "1..*" Noticia : news
```
