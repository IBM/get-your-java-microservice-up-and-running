# Configure the IBM Cloud Container Registry

### STEP 1: Select in **Kubernetes** the entry **Registry** and ensure your are in the **Dallas location**.

![](../../images/ibmcloud-configure-container-registry-1.gif)

### STEP 2: The create a namespace with a unique name cloud-native-[YOURNAME]

![](images/ibmcloud-configure-container-registry-2.gif)

_Note:_ Namespaces are required to be **unique** across the entire **region** that the **specific registry** is located in, not just **unique to your account**. This is mentioned in the following [public documentation](https://cloud.ibm.com/docs/services/Registry?topic=registry-getting-started#gs_registry_namespace_add).

---

Now we have created a free IBM Kubernetes Cluster and we configured the IBM Cloud Container Registry.

---
