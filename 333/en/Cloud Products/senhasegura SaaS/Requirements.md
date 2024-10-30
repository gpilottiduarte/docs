# Requirements

For a successful implementation and operation of senhasegura's solutions in both the standard SaaS and Private SaaS models, it is essential to meet specific technical and operational requirements. Adhering to these prerequisites will ensure optimal performance, security, and user satisfaction.

## General requirements for both SaaS models

### Compatible Bandwidth for workload

Customers using either the senhasegura standard SaaS or Private SaaS models should have network bandwidth compatible with their intended workloads. Adequate bandwidth is crucial for efficient data transfer between the customer’s environment and the hosting infrastructure, minimizing latency, and enhancing user experience. Key considerations include:

* The number of simultaneous users accessing the platform.  
* The volume of data to be transferred.  
* The complexity of tasks and operations performed.

Conducting a thorough analysis of bandwidth requirements is recommended before deployment to prevent slow loading times and ensure a seamless user experience.

### **Network Connector Agent**

The [installation of the Network Connector](/v3-32/docs/en/network-connector-install) Agent is crucial for both the standard and Private SaaS models. This agent, which will be provided by senhasegura, plays a critical role in establishing a secure and reliable connection with the hosted application. Important considerations include:

* **Secure connection**: ensures data integrity and privacy during transmission.  
* **Proper installation**: required for the application’s security and flawless operation.

---

## Optional requirements for Remote Desktop Services server (RDS)

### **Operational System**

For customers who choose to implement a Remote Desktop Services (RDS) server, the following operational system requirements must be met:

* The RDS server should run on Windows Server 2008 R2 or a more recent version.

### **Licensing**

* It is recommended to use RDS Per User CALs (Client Access Licenses) for user or server licenses accessing the RDS.  
* Licensing and implementation must comply with [Microsoft’s terms](https://learn.microsoft.com/en-us/windows-server/remote/remote-desktop-services/rds-client-access-license). Please note that senhasegura does not handle licensing; clients need to acquire licenses directly from Microsoft.

### **Hardware Requirements**

Hardware specifications for the RDS server may vary based on specific workloads and required features. For detailed guidance on hardware specifications, consult [Microsoft's Remote Desktop Workloads documentation](https://learn.microsoft.com/en-us/windows-server/remote/remote-desktop-services/virtual-machine-recs#workloads).

By fulfilling these requirements, organizations can ensure a consistent and effective operation of senhasegura's standard and Private SaaS solutions, maximizing the benefits of identity protection and management.

