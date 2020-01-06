## 2.10

Fixed already in 2.8. No additional changes made here.

[docker-compose.yml](../2.8/docker-compose.yml)

Changes:
* Removed `API_URL` and `FRONT_URL` environment variables from frontend and backend. They are correct by default.
* Removed exposing ports in front- and backend, exposed nginx instead
