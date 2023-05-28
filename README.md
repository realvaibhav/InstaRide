# Instaride

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://github.com/realvaibhav/InstaRide)
[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/realvaibhav/InstaRide)
[![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/realvaibhav/InstaRide)
[![size](https://img.shields.io/github/repo-size/realvaibhav/InstaRide?style=flat-square)](https://github.com/realvaibhav/InstaRide)
[![Website status](https://img.shields.io/website-up-down-green-red/http/shields.io.svg)](https://github.com/realvaibhav/InstaRide)

Many apps rely on real-time, bi-directional communication to give users a great experience. One example is a ride-sharing app like Uber or Lyft, which is built on the messages that are sent between a rider and a driver. A rider selects a starting location and destination, and then the app broadcasts a trip request to all nearby drivers. An available driver accepts the trip and meets the rider at the pick-up address. In the meantime, every move the driver makes is sent to the rider almost instantaneously and the rider can track the trip status as long as it is active.

## Setup

```bash
git clone https://github.com/realvaibhav/InstaRide.git insta
cd insta
docker-compose up
```

## Collections

![db](https://user-images.githubusercontent.com/56718659/234960915-1bc22e07-7bcd-469c-8ef5-2114b0ac03dc.png)

## Dependencies

| Dependency | Version |
| --- | --- | 
| Python | 3.10 | 
| Django | 4.1 |
| Django Channels | 4.0 |
| Django REST Framework | 3.14 |
| pytest | 7.2 |
| Redis | 7.0 |
| PostgreSQL | 15.0 |
| Node | v20 |
| React | v18.2 |
| CRA | v5.0 |
| Docker Engine | v20.10 |
| Docker Compose | v2.12 |
| Tailwind | 2.0 |

## Routes

| Path            | Component        | Functionality                      |
| --------------- | ----------------- | ------------------------------------ |
| /               | Landing           | Renders the landing page.            |
| /sign-up        | SignUp            | Renders the sign-up form.            |
| /log-in         | LogIn             | Renders the log-in form.             |
| /rider          | Rider             | Renders the rider dashboard.         |
| /rider/request  | RiderRequest      | Renders the rider request form.      |
| /rider/:id      | RiderDetail       | Renders details of a specific ride.  |
| /driver         | Driver            | Renders the driver dashboard.        |
| /driver/:id     | DriverDetail      | Renders details of a specific driver. |

## Endpoints

| Endpoint                  | HTTP Method | CRUD Method | Result                                          |
| ------------------------- | -----------| ------------| ----------------------------------------------- |
| /admin/                   | GET        | READ        | Django's built-in admin site.                   |
| /api/sign_up/             | POST       | CREATE      | JSON response with a token.                     |
| /api/log_in/              | POST       | CREATE      | JSON response with a token.                     |
| /api/token/refresh/       | POST       | CREATE      | JSON response with a new token.                 |
| /api/trip/                | GET        | READ        | JSON response with a list of all `Trip` objects.|
| /api/trip/<uuid:trip_id>/ | GET        | READ        | JSON response with the specified `Trip` object. |

##UI/ScreenShots

![Screenshot from 2023-05-12 01-58-03](https://github.com/realvaibhav/InstaRide/assets/56718659/89c3bbea-33c6-4ff9-8499-92650577527c)
![Screenshot from 2023-05-12 01-57-32](https://github.com/realvaibhav/InstaRide/assets/56718659/146b019c-1259-486e-8729-27a9ce309bd2)
![Screenshot from 2023-05-12 01-57-18](https://github.com/realvaibhav/InstaRide/assets/56718659/8e005578-0c34-47f4-b518-97b1a878d1e6)
![Screenshot from 2023-05-12 01-57-07](https://github.com/realvaibhav/InstaRide/assets/56718659/36b2f908-d11b-4cba-afb1-d2d56b747e42)
![Screenshot from 2023-05-12 01-56-48](https://github.com/realvaibhav/InstaRide/assets/56718659/ff315f30-178d-4699-8cc2-3c0e7e8f7270)
![Screenshot from 2023-05-12 01-56-05](https://github.com/realvaibhav/InstaRide/assets/56718659/2d9457bc-ea40-46d0-a285-325e6b83a68e)
![Screenshot from 2023-05-11 23-27-04](https://github.com/realvaibhav/InstaRide/assets/56718659/fd7231f6-fc36-4d46-8aa6-89d8e93976b6)
![Screenshot from 2023-05-11 23-26-13](https://github.com/realvaibhav/InstaRide/assets/56718659/9e308371-e994-44d6-a202-6593bc9a7ea3)
![Screenshot from 2023-05-11 23-24-15](https://github.com/realvaibhav/InstaRide/assets/56718659/b9a9077d-1608-4d76-9dd7-ef65245090d5)
![Screenshot from 2023-05-11 23-11-35](https://github.com/realvaibhav/InstaRide/assets/56718659/1d06d231-adc7-4d96-9f78-09875b70c7af)
![Screenshot from 2023-05-11 23-10-41](https://github.com/realvaibhav/InstaRide/assets/56718659/95465452-b684-4d44-bdda-84f40309c900)
![Screenshot from 2023-05-11 23-09-51](https://github.com/realvaibhav/InstaRide/assets/56718659/28af27f0-4ba3-47df-a22c-4524c8b9493f)
![Screenshot from 2023-05-11 23-05-46](https://github.com/realvaibhav/InstaRide/assets/56718659/10a4c450-9003-4313-947c-3d4469f8e21e)
![Screenshot from 2023-05-11 23-05-19](https://github.com/realvaibhav/InstaRide/assets/56718659/51455d39-f5e5-40b8-8b6f-4f7b4b09dd49)
![Screenshot from 2023-05-11 23-03-59](https://github.com/realvaibhav/InstaRide/assets/56718659/55f16c6b-9e68-4a8a-88f8-d9eaa489e566)
