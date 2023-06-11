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

## UI/ScreenShots

Sign Up form for Rider/Customer
![Screenshot from 2023-05-11 23-03-59](https://github.com/realvaibhav/InstaRide/assets/56718659/35d3f3e9-fee9-4a46-b347-3bb8e66e22d8)
Log In for Rider
![Screenshot from 2023-05-11 23-05-19](https://github.com/realvaibhav/InstaRide/assets/56718659/db2edf9a-3006-4504-b3fb-cd8d4e620260)
Sign Up form for Driver
![Screenshot from 2023-05-11 23-24-15](https://github.com/realvaibhav/InstaRide/assets/56718659/52aecf3a-62f1-4a43-8dcf-90df13050d68)
Log In for Driver
![Screenshot from 2023-05-11 23-09-51](https://github.com/realvaibhav/InstaRide/assets/56718659/5a81a8cd-530b-4ad9-b5dd-91eb08a04695)
Rider Dashboard
![Screenshot from 2023-05-11 23-05-46](https://github.com/realvaibhav/InstaRide/assets/56718659/54b08d40-6e46-4053-8d61-7e9acc13faaa)
Request a Ride
![Screenshot from 2023-05-11 23-10-41](https://github.com/realvaibhav/InstaRide/assets/56718659/d7d668e0-01d3-45f7-aa81-b7277b2b5c48)
Enter the location credentials
![Screenshot from 2023-05-11 23-26-13](https://github.com/realvaibhav/InstaRide/assets/56718659/6b377dcf-8856-4050-9e67-32f0fb24a774)
Driver received the request


![Screenshot from 2023-05-11 23-27-04](https://github.com/realvaibhav/InstaRide/assets/56718659/8402638b-1dd8-4ba8-acb2-30f037c23054)


Driver Dashboard
![Screenshot from 2023-05-12 01-56-05](https://github.com/realvaibhav/InstaRide/assets/56718659/512768f7-a7db-408b-9e50-baf78d5ae103)
Rider starts the journey with Driver
![Screenshot from 2023-05-12 01-57-07](https://github.com/realvaibhav/InstaRide/assets/56718659/923529d8-53ec-49b2-9fe8-88fffcd05faa)

![Screenshot from 2023-05-12 01-57-18](https://github.com/realvaibhav/InstaRide/assets/56718659/64ba920a-470a-48dd-88b3-f98d6e2ca2b2)
Ride Completed
![Screenshot from 2023-05-12 01-57-32](https://github.com/realvaibhav/InstaRide/assets/56718659/acb87ca0-e7de-4aa4-b2d4-d7019819c3ab)
Ride Added to recent trips
![Screenshot from 2023-05-12 01-58-03](https://github.com/realvaibhav/InstaRide/assets/56718659/a349026d-06c0-46a8-a36e-9285c58ba417)


