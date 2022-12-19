# Status (testausserveri)

**!!! THERE IS NO AUTODEPLOY FOR THIS REPO! ASK ROY TO DEPLOY THIS! !!**

This is [testausserveri](https://testausserveri.fi)'s status page configuration. 


**Status pages:**
- [official](https://status.testausserveri.fi)
- [members](https://members.status.testausserveri.fi)

## What is this

This repository contains the docker-compose files and gatus configurations for the service. They can be pulled from this repo to initialize the server. Later a cron job can be added to pull the changes periodically.

## Initialize

Deploy to a server:

```sh
ansible-playbook deploy.yml -i inventory.ini
```