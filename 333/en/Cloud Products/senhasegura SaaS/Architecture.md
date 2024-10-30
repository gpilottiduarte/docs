# Architecture

The architecture of senhasegura's solutions is designed to provide flexible, secure, and scalable options to meet the diverse needs of clients. By offering both Private SaaS and standard SaaS models, senhasegura ensures that organizations can choose the architecture that best fits their security, compliance, and operational requirements.

## Data center location and security

senhasegura's SaaS application is operated from Google's secure third-party data centers that boast SOC 2 Type II and SOC 3 Type II certification. These centers are equipped with robust backup power systems, fire suppression mechanisms, and round-the-clock security personnel. Physical access to server rooms is highly restricted, ensuring stringent control over intrusions.

To comply with local regulations such as GDPR and respect national sovereignty, each client's tenant is hosted on geographically proximate servers, ensuring compliance and low-latency performance.

### Geographical availability for SaaS

* **Brazil**  
* **USA (Coming Soon)**  
* **Europe (Coming Soon)**  
* **Middle East (Coming Soon)**

### Geographical availability for Private SaaS 

* **Any region offered by GCP (Google Cloud Platform).**

## Communication and integration

All communication between senhasegura and the client's corporate network is facilitated through the [Network Connector](/v3-33/docs/network-connector). This connector is implemented as a container that integrates seamlessly with the client's existing network infrastructure.

---

## VPN-less architecture

![image](https://cdn.document360.io/5a1d58df-64ce-42a2-8b23-688477d32f33/Images/Documentation/image-1689002215816.png){height="" width=""}

In the VPN-less model, all connectivity inside customer environment is managed via the Network Connector. Key characteristics include:

* The senhasegura instance may or may not be publicly accessible.  
* Users access senhasegura using the client's public IP address.  
* Clients can authorize multiple IP addresses for accessing the senhasegura GUI.

**Note:** Connections to senhasegura are made via the internet. If the client has a way to identify the public IPs from which connections will be made, we can filter only those IPs to enhance security. This includes clients with a range of IP addresses contracted from their ISP or those mapping each outgoing IP individually.

### Using senhasegura Network Connector

senhasegura offers a [Network Connector](https://docs.senhasegura.io/v3-33/docs/network-connector) that can be deployed within a customer's infrastructure. This connector facilitates various tasks such as remote password changes, acts as a proxy for remote access connections, and enables integration with other customer services. It is a critical component for maintaining secure connectivity between the customer’s environment and senhasegura’s SaaS solutions.

### Using senhasegura Go Endpoint Manager

All communication with the senhasegura Go Endpoint Manager is conducted via HTTPS, ensuring secure connectivity. Managed endpoints are required to have the capability to connect to senhasegura's SaaS tenant.

---
