# jhipster-gitlab-ci
---

## Description
This project builds a docker image _FROM jhipster/jhipster_ (Official JHipster Docker image)
 - Refer to https://hub.docker.com/r/jhipster/jhipster/ and https://jhipster.github.io/ for more information
 - Dockerfile is fairly simple, we use the 'root' user instead of the 'jhipster' user defined in jhipster docker image 


## Intended usage
As part of Jhipster microservice-oriented development, you may decide to separate your front-office from your back-office.<br>
While building your front-office, you can encounter right issues during the building steps (gulp build), because Gitlab checks out source files as root (unless specified differently). <br>
If you use jhipster docker image to build, the user 'jhipster' will deal with files belonging to 'root', hence right issues.
 