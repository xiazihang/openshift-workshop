title: Openshift Workshop
speaker: Zihang
url: https://github.com/ksky521/nodePPT
transition: zoomin 
files: /js/demo.js,/css/demo.css
theme: light

[slide style="background-image:url('/img/bg1.png')"]

# Openshift Workshop
## Zihang & Lixuan

[slide style="background-image:url('/img/bg1.png')"]

# Openshift Origin Overview 

--- 

- Based on Kubernates and Docker {:&.moveIn}
  * Docker: packging, creating linux-based and lightweight container image, running containerized application {:&.moveIn}
  * Kubernates: cluster management and orchestrates containers on multiple hosts 
- Source Control Management 
  * Integrate with preexisting SVC(only support Git for now) {:&.moveIn} 
  * Webhook: Triggers build upon repository changes 
- Managing images  
  * Container registry {:&.moveIn}
- Application management 
  * Building {:&.moveIn} 
  * Deployment 
  * Self-healing 
  * Auto-scaling 

[slide]

# Openshift Origin Infrustracture 

--- 

![infrustracture](/img/openshift-infrastructure.png) 

[slide]

# Core Concepts 

--- 

- Container and Images 
- Pods and Services 
- Projects 
- Builds  
- Deployment 

[slide ]

# Core Concepts 

---
- Container and Images {:&.moveIn} 
    - Container: Docker-formatted container {:&.moveIn}
    - Image: include all requirements of running a container  
    - Container Registries: Docker Hub, private registry, third-party regitry 

[slide]

# Container registry 

---

![registry](/img/container-registry.png) 

[slide]

# Core Concepts 

---
- Pods and Services {:&.moveIn}
  - Pods: a set of one or more containers, smallest compute unit can be defined, deployed and managed {:&.moveIn}
  - Services: internal loadbalancer, expose backing pods service to external clients 
  - labels
[slide]

# Pods and Services {:&.flexbox.vleft}  

![pods](/img/services.jpeg) 

[slide]

# Core Concepts

---

- Projects 
  - namespace: machanism to scope resources in cluster {:&.moveIn} 


[slide]

# Core Concepts 

---

- Build 
  - BuildConfig {:&.moveIn} 

[slide]

# BuildConfig 

---

![buildconfig](/img/buildconfig.png)

[slide]

# Core Concepts 

---

- Deployment 

  - deployment configuration {:&.moveIn}
  - Replication Controller  
  - one or more pods 


[slide]

# DeployConfig 

---

![deployconfig](/img/deployconfig.png) 

[slide]

# Practice Part1

- Content:

    - A simple nodejs application 
    - Add mongodb to the application 

- Preparation
    - Install `oc` in your mac:
```
brew update 
brew install openshift-cli 
oc version # check oc version => 1.5+
```
    - fork the demo project(https://github.com/openshift/nodejs-ex) to your own github account 
    - Clone configuration files
    ```
    git clone https://github.com/xiazihang/openshift-workshop.git 
    ```
