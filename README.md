# weather-station-db

## Build and Run with Docker

- `docker build -t tutum/influxdb .`
- `docker run -d -p 8083:8083 -p 8086:8086 tutum/influxdb`
- additional params:
  - add persistent volume `-v=/var/influxdb:/data`
  - change admin user `-e ADMIN_USER="root" -e INFLUXDB_INIT_PWD="somepassword"`
- open http://localhost:8083 in browser for admin console
- client server connection is available over port **8086**
