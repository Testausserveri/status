# gatus-deployer
This is [testausserveri](https://testausserveri.fi)'s status page configuration. 


**Status pages:**
- [official](https://status.testausserveri.fi)
- [members](https://members.status.testausserveri.fi)

## What is this

This repository contains the docker-compose files and gatus configurations for the service. They can be pulled from this repo to initialize the server. Later a cron job can be added to pull the changes periodically.

## Initialize

I would recommend placing this repo to `/opt` directory.

It would happen followingly:

```sh
cd /opt
git clone https://github.com/RoyTakanen/status.git
```

To finish things I would also add a cron job that would pull the changes on the repo and redeploy the stack.

```sh
* * * * * cd /opt/status && git pull && docker-compose up -d
```