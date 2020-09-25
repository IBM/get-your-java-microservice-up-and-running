# Using local Code and the prebuilt Docker image with the Code in the Container 

### STEP 1: Code locally - Open a terminal session and run these commands

Download the project locally to work in the Developer labs locally.

```sh
git clone https://github.com/IBM/cloud-native-starter
cd cloud-native-starter
ROOT_FOLDER=$(pwd)
```

The local project is needed for Java development labs 2 and 3, because you can't use Docker in the 'cns-workshop-tools' Docker image. (for more see this [article](https://suedbroecker.net/2019/08/27/definition-of-a-dockerfile-to-use-bash-scripts-on-a-windows-10-machine-for-our-cloud-native-starter-workshop/) )

### STEP 2: Open new terminal session and run these commands

* Start the container

```
docker run -it --rm tsuedbroecker/cns-workshop-tools:v3
```

### STEP 3: After the container has been started, run these commands inside your running Docker image to get the lastest version of the workshop:

```
cd /
git clone https://github.com/IBM/cloud-native-starter.git
cd cloud-native-starter
ROOT_FOLDER=$(pwd)
```

### STEP 4: Verfiy the tool prerequisites on for the workshop

```
chmod u+x iks-scripts/*.sh
chmod u+x scripts/*.sh
./iks-scripts/check-prerequisites.sh
```

---

