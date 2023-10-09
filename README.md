
## Description
Ticketing System using NEST JS. 
- Class Diagram

```mermaid
classDiagram
  class organization{
    +name String
    +description String
    +address String
  }
  class user{
    +name String
    +email String
    +password String
    +role String
    +organization String
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
  event <|-- booking
  user <|-- booking
  organization <|-- user
```

## Installation

```bash
$ npm install
```

## Running the app

```bash
# development
$ npm run start
```
## Build the app
```bash
$ npm install
$ npm run build # both ReactJS and NestJS
$ npm run build:backend # only NestJS backend
$ npm run build:frontend # only ReactJS frontend
```
## Test

```bash
$ npm run test # run project tests under `cypress/integration`
```

