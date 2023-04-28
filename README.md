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
