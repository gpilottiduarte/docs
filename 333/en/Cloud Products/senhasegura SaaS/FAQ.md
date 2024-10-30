# FAQ

## **Updates and maintenance**

### **Instance snapshots**

* **Who is responsible for taking snapshots of the instance?**  
  * senhasegura is responsible for taking these snapshots daily and before scheduled maintenance.

### **Version updates**

* **How are version updates conducted?**  
  * In the SaaS model, updates are handled by support according to the manufacturer’s schedule. In the Private SaaS model, updates are coordinated between the support team and the client.

## **Architecture and backup**

### **Snapshots Vs. Regular backups**

* **Why are snapshots taken instead of regular backups?**  
  * Snapshots capture a complete image of the application, allowing for restoration in the event of unavailability or an incident.

### **Local backup**

* **Why is there a local backup?**  
  * Local backups allow for “break the glass” procedures without requiring access to the cloud, ensuring device access during unavailability.

### **Backup storage**

* **Where are the backup copies stored?**  
  * Credential backups are stored on the client's network for "break the glass" procedures.

### **Cloud provider options**

* **Can I use another cloud provider?**  
  * senhasegura defines the service provider for SaaS. Clients preferring a different provider must opt for the on-premises version.

### **Redundancy and Disaster Recovery**

* **Is there redundancy between different regions?**  
  * By default, no. senhasegura uses Google's contingency services for data availability. Multi-region architectures require an additional service contract.  
* **Is it possible to have a Disaster Recovery instance on another cloud?**  
  * DR environments aren't typically included by default in senhasegura offerings; they involve extra costs and complex arrangements.

### **Active-Active architecture**

* **Is an active-active architecture available?**  
  * Google's environment includes region-specific backup systems. Inter-region backup services are available separately.

### **Custom backup configurations**

* **Is it possible to create backups on other cloud providers?**  
  * Customers can back up videos and credentials on a personally managed server, be it cloud-based or physical. Daily snapshots by senhasegura are stored on GCP in the same region as the instance.

## **Regulations and security**

### **Contingency plans**

* **What is the contingency plan in the event of a failure in the hosted region?**  
  * GCP's multiple data centers within each region ensure transparent failovers, minimizing failure risks.

### **Intrusion testing**

* **How often are intrusion tests conducted in the application environment?**  
  * Intrusion tests coincide with each software update in the hosting environment, utilizing market-standard tools and external consultants.

### **Data security**

* **What ensures that the client machine won’t be cloned or copied?**  
  * senhasegura employs comprehensive operational policies certified by ISO 27001 to prevent errors.

## **Remote management and access**

### **Support access**

* **How does senhasegura provide remote support for SaaS customers?**  
  * Access by the senhasegura team is limited to the client's network, with all activities logged for audit trails.

### **Orbit panel access**

* **Is there access to the Orbit panel in SaaS?**  
  * In the new SaaS model, only senhasegura can access the Orbit menu. Clients have Orbit access in the Private SaaS setup.

## **Backup management**

### **Responsibility for backups**

* **Who manages the backups in SaaS and Private SaaS?**  
  * In the SaaS model, senhasegura manages system backups, while password backups fall to the client via rsync. Private SaaS clients manage both system and password backups independently.

