# Overview

We are using caddy as sidecar with ssl to then re-route users to our docker container for our registry at port 5000.

# Start
```
docker compose up -d
```

# List repositories
From within the host:
`curl localhost:5000/v2/_catalog`
Or from outside, have to hit the reverse proxy first.

