title: Openshift Workshop
speaker: Zihang
url: https://github.com/ksky521/nodePPT
transition: zoomin 
files: /js/demo.js,/css/demo.css

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
  * Image stream 
  * Image tag policy  
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
- deployment 

[slide ]

# Core Concepts 

---
- Container and Images {:&.moveIn} 
    - Container: Docker-formatted container {:&.moveIn}
    - Image: include all requirements of running a container  
    - Container Registries: Docker Hub, private registry, third-party regitry 

[slide style="background-image:url('/img/container-registry.png')"]

[slide]

# Core Concepts 

---
- Pods and Services {:&.moveIn}
  - Pods: a set of one or more containers, smallest compute unit can be defined, deployed and managed {:&.moveIn}
  - Serivces: internal loadbalancer, expose backing pods service to external clients 
  - labels
[slide]

# Pods and Services {:&.flexbox.vleft}  

![pods](/img/services.jpeg) 

[slide]

# Core Concepts

---

- Projects 
  - namespace: machanisam to scope resources in cluster {:&.moveIn} 


[slide]

# Core Concepts 

---
- Builds 
  - BuildConfig {:&.moveIn}

[slide]

# Core Concepts 

---

- Deployments 
  - Replication Controller 


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
    git clone https://github.com/gmlove/openshift-workshop.git 
    ```
