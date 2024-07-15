#Santander Dev Week 2024
Java RESTful API criada para a dev week do Santander.

##Diagrama de Classes

'''mermaid
classDiagram
    class User {
        -String name
        -Account account
        -Features[] features
        -Card card
        -News[] news
    }

    class Account {
        -String number
        -String agency
        -BigDecimal balance
        -BigDecimal limit
    }

    class Features {
        -String icon
        -String description
    }

    class Card {
        -String number
        -BigDecimal limit
    }

    class News {
        -String icon
        -String description
    }

    User "1" *-- "1" Account
    User "1" *-- "n" Features
    User "1" *-- "1" Card
    User "1" *-- "n" News
'''
