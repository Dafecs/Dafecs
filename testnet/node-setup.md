# Node Setup

## Super Easy To Run a Node <a id="super-easy-to-run-a-node"></a>

You can either run a node:

* Via deploy to a host in the cloud
* On any machine with Docker installed

## One Liner Deploy Script To The Cloud <a id="one-liner-deploy-script-to-the-cloud"></a>

### Requirements <a id="requirements"></a>

* A Mac or Linux shell environment
* curl with ssl support

### ​ <a id="undefined"></a>

### Digital Ocean <a id="digital-ocean"></a>

**Prerequisites**: Follow these instructions to [signup for a Digital Ocean account](https://www.digitalocean.com/docs/getting-started/sign-up/). You need a Digital Ocean [API token](https://www.digitalocean.com/docs/apis-clis/api/create-personal-access-token/). You may export your token as the env var `DIGITALOCEAN_ACCESS_TOKEN` or simply provide it when script asks for it.

#### **One Liner Install For Digital Ocean** <a id="one-liner-install-for-digital-ocean"></a>

```text
bash -c "$(curl -fsSL https://dafecs.com/one-click-DO.sh)"
```

Each run of this script will generate a Droplet on Digital Ocean running a Dafecs node. You will receive an email to the address used in your Digital Ocean registration with login credentials. The Dafecsnode runs as a docker image.

## Running using Docker Compose <a id="running-using-docker-compose"></a>

**Step 1:** Download the [docker-compose.yml](https://raw.githubusercontent.com/Dafecs-project/dafecs-ops/master/scripts/docker-compose.yml) file to your machine that has Docker installed.

**Step 2:** Start the node

You can also start the node as a detached background service:

To view the logs you then use the docker logs command:

```text
docker logs dafecs-node -f
```

