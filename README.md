
## Description
Ticketing System using NEST JS. 
1. Class Diagram

```mermaid
classDiagram
  class user{
    +name String
    +email String
    +password String
    +role String
  }
  class event{
    +name String
    +location String
    +start_date DateTime
    +end_date DateTime
    +ticket_qty Int
  }
  class booking{
    +user User
    +event Event
    +booking_no String
    +ticket_qty Int
    +payment_no String
    +status String
  }
  Event <|-- Booking
  User <|-- Booking
```

## Installation

```bash
$ npm install
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

