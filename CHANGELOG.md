# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html). (Patch version X.Y.0 is implied if not specified.)

## [Unreleased]
### Added
- isuftin@usgs.gov - Added wait-for.sh (and the netcat package) to help with
downstream container start orchestration
- kmschoep@usgs.gov - Dockerfile
- kmschoep@usgs.gov - docker-compose.env
- kmschoep@usgs.gov - docker-compose.yml
- kmschoep@usgs.gov - .travis.yml
- isuftin@usgs.gov - python user
- isuftin@usgs.gov - curl check in travis to verify http server is running
- isuftin@usgs.gov - certificate import script
- isuftin@usgs.gov - maintainer label in Dockerfile
- isuftin@usgs.gov - certificate import envs in Dockerfile
- isuftin@usgs.gov - sample application for base container
- isuftin@usgs.gov - health check
- isuftin@usgs.gov - onbuild command to remove sample application on downstream containers
- isuftin@usgs.gov - squelching pip installation

### Changed
 - isuftin@usgs.gov - use port 8000
 - isuftin@usgs.gov - switch in entrypoint to test for sample application
 - isuftin@usgs.gov - Moved lines around in Dockerfile
 - isuftin@usgs.gov - Dockerfile now uses python user instead of root
 - isuftin@usgs.gov - Removed check in travis for a running container
 - isuftin@usgs.gov - Split out config to config.env and secrets.yml
 - isuftin@usgs.gov - docker-compose now mounts certificates into python home dir
