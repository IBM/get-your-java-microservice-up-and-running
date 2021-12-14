# Using local Code and the prebuilt Docker image with the Code in the Container

## Step 1: Code locally - Open a terminal session and run these commands

Download the project locally to work in the Developer labs locally.

```sh
git clone https://github.com/IBM/cloud-native-starter
cd cloud-native-starter
ROOT_FOLDER=$(pwd)
```

The local project is needed for Java development labs 2 and 3, because you can't use Docker in the 'cns-workshop-tools' Docker image. (for more see this [article](https://suedbroecker.net/2019/08/27/definition-of-a-dockerfile-to-use-bash-scripts-on-a-windows-10-machine-for-our-cloud-native-starter-workshop/) )

### Step 2: Open new terminal session and run these commands

* Start the container

```bash
docker run -it --privileged --rm quay.io/tsuedbroecker/cns-workshop-tools:buildah-v1
```

### Step 3: After the container has been started, run these commands inside your running Docker image to get the lastest version of the workshop

```bash
cd /
git clone https://github.com/IBM/cloud-native-starter.git
cd cloud-native-starter
ROOT_FOLDER=$(pwd)
```

### Step 4: Verfiy the tool prerequisites on for the workshop

```bash
chmod u+x iks-scripts/*.sh
chmod u+x scripts/*.sh
./iks-scripts/check-prerequisites.sh
```

---
