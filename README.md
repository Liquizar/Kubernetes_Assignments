# 🌟 Kubernetes Assignments 🌟

This repository contains solutions to a series of Kubernetes assignments. Each assignment demonstrates various Kubernetes concepts and functionalities. Below is a detailed description of each assignment and the corresponding folder structure.

## 📂 Folder Structure

```
.
├── Assignment1_nginx
│   ├── nginx-deployment.yaml
|   └── README.md
├── Assignment2_wordpress-kustomize
│   ├── kustomization.yaml
│   ├── mysql-deployment.yaml
|   ├── secret.yaml
│   ├── wordpress-deployment.yaml
|   └── README.md
├── Assignment3_loopback
│   ├── k8s
│   ├── loopback4-example-todo
|   └── README.md
├── Assignment4_simple-webapp
│   ├── k8s
│   ├── app.py
│   ├── Dockerfile
│   ├── requirements.txt
|   └── README.md
├── Assignment5_multi-container-pod
│   ├── multi-container-pod.yaml
|   └── README.md
├── Assignment6_nginx-deployment
│   ├── nginx-deployment.yaml
│   ├── nginx-service.yaml
|   └── README.md
|
└── README.md
```

## 📜 Assignment Details

### Assignment 1: Nginx Deployment and Rolling Update 🚀

**Folder:** `Assignment1_nginx`

1. **Create a Deployment:**
   - Deploy nginx version 1.7.9 with 3 replicas.

2. **Perform a Rolling Update:**
   - Update the deployment to nginx version 1.9.1.

**Files:**
- `nginx-deployment.yaml`: Contains the Kubernetes manifest for the nginx deployment and the rolling update configuration.

### Assignment 2: WordPress and MySQL with Kustomize 🖥️

**Folder:** `Assignment2_wordpress-kustomize`

1. **Create PersistentVolumes and PersistentVolumeClaims.**
2. **Create a `kustomization.yaml` with:**
   - A Secret generator.
   - MySQL resource configurations.
   - WordPress resource configurations.

3. **Apply the kustomization directory and verify objects:**
   - ✅ Verify the Secret.
   - ✅ Verify PersistentVolume provisioning.
   - ✅ Verify the Pod and Service.
   - 🌐 Access WordPress site via IP address.

**Files:**
- `kustomization.yaml`
- `secret.yaml`
- `mysql-deployment.yaml`
- `wordpress-deployment.yaml`

### Assignment 3: LoopBack Application Deployment 🔄

**Folder:** `Assignment3_loopback`

1. **Get the LoopBack "Getting Started" App:**
   - Clone the repository: `git clone https://github.com/strongloop/loopback-getting-started`.

2. **Create a Dockerfile:**
   - Create a Dockerfile in the application directory.

3. **Build and Publish the Image:**
   - Build the Docker image and tag it for your Docker registry.

4. **Create a Deployment Manifest:**
   - Create `app.yml` for the application deployment.

5. **Test the Deployed Application:**
   - Access the application at `https://127.0.0.1/testapp`.

**Folders:**
- `k8s`
- `loopback4-example-todo`

### Assignment 4: Web Application Service 🌐

**Folder:** `Assignment4_simple-webapp`

1. **Create a Service to Access the Web Application:**
   - Define the service in `service-definition-1.yaml`.

**Files and Folders:**
- `k8s`
- `app.py`
- `Dockerfile`
- `requirements.txt`

### Assignment 5: Multi-Container Pod 🐳

**Folder:** `Assignment5_multi-container-pod`

1. **Create a Multi-Container Pod:**
   - Define the pod with two containers: `lemon` (busybox) and `gold` (redis).
   - Handle crashloopbackoff by adding `sleep 1000` to `lemon` container if necessary.

**Files:**
- `multi-container-pod.yaml`

### Assignment 6: Nginx Deployment with Service 🌍

**Folder:** `Assignment6_nginx-deployment`

1. **Create a Deployment:**
   - Deploy nginx and expose it via a ClusterIP service.

**Files:**
- `nginx-deployment.yaml`
- `nginx-service.yaml`


## 🚀 How to Use

1. Clone the repository:
   ```sh
   git clone https://github.com/Liquizar/Kubernetes_Assignments.git
   cd Kubernetes_Assignments
   ```

2. Navigate to the respective assignment folder and apply the Kubernetes manifests using `kubectl apply -f <filename>`.

3. Follow the instructions provided in each assignment section to verify and test the deployments.

Feel free to explore each folder for detailed Kubernetes manifests and configurations. If you have any questions or need further assistance, please open an issue in this repository.
