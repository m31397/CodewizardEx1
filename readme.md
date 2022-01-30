# 1st Exercise

## Required
- [docker](https://docs.docker.com/get-docker/)

## Usage

### Installation

Use [docker](https://docs.docker.com/get-docker/) to install and run Jenkins.

```sh
docker-compose up -d
```

### Dashboard

In order to enter the Jenkins Dashboard just enter `localhost` or `127.0.0.1` in your browser.

## Jenkins Configuration Examples

### Change default users

Change the `casc.yaml` file.


```yaml
jenkins:
  securityRealm:
    local:
      allowsSignup: false
      users:
       - id: test1
         password: test1
       - id: test2
         password: test2
```