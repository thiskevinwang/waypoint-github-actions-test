This repository is a proof-of-concept for...

1. Using [`waypoint`][waypoint] in GitHub actions
   - Using a Waypoint server hosted on [HCP](https://portal.cloud.hashicorp.com/)
   - Using a GitHub actions runner as a Waypoint runner
1. Building [`waypoint-plugin-nixpacks`][wpn] in GitHub actions
1. Using [`waypoint`][waypoint] + [`waypoint-plugin-nixpacks`][wpn] to build a sample app, and publish the build image to [DockerHub](https://hub.docker.com/r/thekevinwang/express-nixpacks-example)

[wpn]: https://github.com/thiskevinwang/waypoint-plugin-nixpacks
[waypoint]: https://developer.hashicorp.com/waypoint
