![CleanShot 2023-02-20 at 21 07 05@2x](https://user-images.githubusercontent.com/26389321/220229432-09dfa2d7-88cb-4bfc-9ed2-29a24fa2c706.png)


This repository is a proof-of-concept for...

1. Using [`waypoint`][waypoint] in GitHub actions
   - Using a Waypoint server hosted on [HCP](https://portal.cloud.hashicorp.com/)
   - Using a GitHub actions runner as a Waypoint runner
1. Building [`waypoint-plugin-nixpacks`][wpn] in GitHub actions
1. Using [`waypoint`][waypoint] + [`waypoint-plugin-nixpacks`][wpn] to build a sample app, and publish the build image to [DockerHub](https://hub.docker.com/r/thekevinwang/express-nixpacks-example)

[wpn]: https://github.com/thiskevinwang/waypoint-plugin-nixpacks
[waypoint]: https://developer.hashicorp.com/waypoint

The [workflow file](./.github/workflows/workflow_dispatch.yml) relies on 4 repository [secrets][secrets] (Note: [variables][variables] can be used for the non-sensitive values):

- `DOCKERHUB_TOKEN`
- `DOCKERHUB_USERNAME` (not sensitive)
- `WAYPOINT_SERVER_ADDR` (not sensitive)
- `WAYPOINT_SERVER_TOKEN`

[secrets]: https://docs.github.com/en/actions/security-guides/encrypted-secrets
[variables]: https://docs.github.com/en/actions/learn-github-actions/variables
