# Deployment of Multi-tier (WordPress + MySQL) application in Kubernetes Cluster

**Objective:** To deploy a multi-tier MySQL application using Kubernetes with specific configurations for user roles, storage, service verification, namespace restrictions, quota limits, and data management.

**Real-time Scenario:** Karen is a DevOps engineer at a tech startup. Her team has developed a new application using MySQL. Now, it is her task to deploy that application. The company plans to utilize Kubernetes for its robust container orchestration capabilities. Karen must create a Kubernetes dashboard with specific configurations, user roles, storage, service verification, and data management.

-------------------------------------------------------------------------------------------------------------------------------------------------

## Major Tools, Environment Used in This Project:

- kubeadm
- kubectl
- kubelet
- Containerd
- Kubernetes Dashboard
- NFS Server

**Pre-requisites:** A Kubernetes cluster should already be set up with 3 Nodes (1 Master and 2 Worker Nodes) using kubeadm.

----------------------------------------------------------------------------------------------------------------------------

## High Level Project Diagram:


<img width="931" height="648" alt="image" src="https://github.com/user-attachments/assets/82f65baa-72e3-4106-ad72-702605de6156" />

----------------------------------------------------------------------------------------------------------------------------------

## High Levels Tasks/Steps:

-	Create Kubernetes Dashboard
-	Install & Configure NFS Server, create NFS based PV & PVC
-	Create Secret for MySQL Deployment
-	Create Deployment for MySQL (attach PV, PVC)
-	Create ConfigMap and Secret for Wordpress Deployment
-	Create Deployment for Wordpress (PV not required)
-	Expose Service for WordPress and MySQL Deployment
-	Verify the Deployment of Application on web browser
-	Verify the Cluster and its workloads on Kubernetes Dashboard

------------------------------------------------------------------------------------------------------------------------------------

## Output Result Screenshots:

Deploying a Kubernetes Dashboard

<img width="917" height="394" alt="image" src="https://github.com/user-attachments/assets/8ba06256-fdad-4c6e-882e-ae69e2d05ac4" />

---------------------------------------------------------------------------------------------------------

Install & Configure NFS Server, create NFS based PV & PVC

<img width="935" height="517" alt="image" src="https://github.com/user-attachments/assets/edf8f3b3-4cce-4453-aaec-783f250196a2" />

------------------------------------------------------------------------------------------

<img width="285" height="366" alt="image" src="https://github.com/user-attachments/assets/a4f0b321-0cab-4505-8602-189bc4e12456" />

--------------------------------------------------------------------------------------------

<img width="368" height="317" alt="image" src="https://github.com/user-attachments/assets/07afecb1-e7ec-41dc-8abf-6fdb0dc3b75d" />

------------------------------------------------------------------------------------------------
Create Deployment for MySQL 

<img width="492" height="990" alt="image" src="https://github.com/user-attachments/assets/df582005-a62b-4981-ad32-def424c23639" />

-------------------------------------------------------------------------------------------------------


MySQL Deployment, pod created in Kubernetes cluster:

<img width="917" height="263" alt="image" src="https://github.com/user-attachments/assets/f56a637f-2580-406e-ac8e-cf94a28c5055" />

-----------------------------------------------------------------------------------------------------------

Expose Service for MySQL Deployment

<img width="965" height="270" alt="image" src="https://github.com/user-attachments/assets/5de64a2f-7740-4f61-8dc3-dd0b3b27136b" />

---------------------------------------------------------------------------------------------------------------

Create Deployment for Wordpress

<img width="529" height="894" alt="image" src="https://github.com/user-attachments/assets/3eead512-6dc0-423c-b213-fd2f28d236e6" />


-------------------------------------------------------------------------------------------------------------------------------------

Wordpress Deployment, pod created in Kubernetes cluster:

<img width="965" height="299" alt="image" src="https://github.com/user-attachments/assets/c11b0a86-1575-4af7-8984-177b29f736ff" />

-------------------------------------------------------------------------------------------------------------------------------------
Expose Service for Wordpress Deployment

<img width="851" height="249" alt="image" src="https://github.com/user-attachments/assets/34b2f275-6606-4a77-b165-8ee90500ddb3" />


------------------------------------------------------------------------------------------------------------------------------------

Verify the Deployment of 2-Tier Application by accessing the Wordpress Application on web-browser:

Access the URL at http://localhost:32658/

<img width="907" height="533" alt="image" src="https://github.com/user-attachments/assets/dbec3a19-bd01-4f06-b9c6-7cbe151ddf19" />

------------------------------------------------------------------------------------------------------------------------------------

<img width="724" height="529" alt="image" src="https://github.com/user-attachments/assets/8a0f2738-4463-4b3a-b8c3-9f217dc70784" />

------------------------------------------------------------------------------------------------------------------------------------

<img width="929" height="501" alt="image" src="https://github.com/user-attachments/assets/60287ef1-e890-4864-ab06-3fca4393edf4" />

------------------------------------------------------------------------------------------------------------------------------------

Verify the Cluster and its workloads on Kubernetes Dashboard.

Access the Kubernetes Dashboard on URL: https://localhost:31855

<img width="945" height="381" alt="image" src="https://github.com/user-attachments/assets/ae2d2255-5b4e-4da0-8673-399af3dbbb61" />

-----------------------------------------------------------------------------------------------------------------------------------

<img width="959" height="513" alt="image" src="https://github.com/user-attachments/assets/4a513b72-7b48-4ce9-8d26-04f42b8cbf8a" />

------------------------------------------------------------------------------------------------------------------------------------

**As per the requirement of the Project: The Deployment of multi-tier application (Wordpress + MySQL) in Kubernetes Cluster has been done successfully.**
**Also, Kubernetes Dashboard has been created to manage and monitor the cluster, workloads and to provide real-time insights from web base GUI.**

