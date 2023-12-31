
## Description
Ticketing System using NEST JS and ReactJS.
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
  }
  class event{
    +name String
    +description String
    +location String
    +start_date DateTime
    +ticket_qty Integer
    +attendees Integer
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
  organization <|-- event
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

