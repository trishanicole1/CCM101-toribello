# Client Recommendations

## Client A – Startup Company

**Scenario:** Launching a new mobile application, limited budget, expects rapid growth.

**Recommended Platform:** AWS

**Justification:**

AWS is a suitable choice for a startup because it offers pay-as-you-go pricing and a range of services that can help control costs during the early stages of development. AWS also provides scalable services that allow the company to increase its computing, storage, and database resources as the number of users grows. Its broad service catalog means the startup can continue using AWS as its application becomes more complex without necessarily needing to migrate to another cloud provider. AWS also has extensive documentation and a large developer community, which can help a small development team find solutions and learn AWS services more easily.

**Services they could use:**

1. **AWS Amplify** – For quickly developing and deploying the backend and supporting services for the mobile application.

2. **Amazon EC2 / AWS Lambda** – For scalable computing. EC2 can provide virtual servers, while Lambda can run application code without requiring the startup to manage servers.

3. **Amazon DynamoDB** – A scalable NoSQL database suitable for applications that need fast and flexible data storage as the user base grows.

4. **Amazon S3** – For storing application assets, images, videos, backups, and other files in scalable cloud storage.

---

## Client B – University

**Scenario:** Already uses Windows Server, Microsoft 365, and Active Directory. Wants to migrate some services to the cloud.

**Recommended Platform:** Microsoft Azure

**Justification:**

Microsoft Azure is a strong choice for the university because it integrates closely with the Microsoft technologies it already uses, including Windows Server, Microsoft 365, and Microsoft Entra ID. This integration can make it easier to manage identities, permissions, applications, and cloud resources without completely replacing the university's existing environment. Azure also supports hybrid cloud deployments, allowing the university to gradually move selected workloads to the cloud while continuing to operate some systems on-premises. This approach can reduce migration risks and allow the university to adopt cloud services at its own pace.

**Services they could use:**

1. **Microsoft Entra ID** – For managing user identities, authentication, permissions, and secure access to cloud applications and resources.

2. **Azure Virtual Machines** – For migrating or hosting Windows Server workloads in the Azure cloud.

3. **Azure Virtual Desktop** – For providing students, faculty, and staff with secure remote access to Windows desktops and university applications.

4. **Azure Files** – For providing managed cloud file shares that can integrate well with Windows-based environments.

---

## Client C – AI Research Company

**Scenario:** Develops AI and Machine Learning applications requiring high-performance computing.

**Recommended Platform:** Google Cloud Platform (GCP)

**Justification:**

Google Cloud Platform is a strong choice for an AI research company because it provides specialized infrastructure and services for artificial intelligence, machine learning, and large-scale data processing. Google Cloud offers access to GPUs and Tensor Processing Units (TPUs), which can provide high-performance computing resources for training and running machine learning models. Vertex AI provides tools for developing, training, deploying, and managing machine learning models throughout the ML lifecycle. Google Cloud also has strong Kubernetes capabilities through Google Kubernetes Engine (GKE), making it suitable for containerized research workloads that need to scale.

**Services they could use:**

1. **Vertex AI** – An end-to-end platform for building, training, deploying, and managing machine learning models.

2. **Compute Engine with GPUs/TPUs** – Provides high-performance computing resources for machine learning training and other computationally intensive workloads.

3. **Google Kubernetes Engine (GKE)** – A managed Kubernetes service for deploying and orchestrating containerized AI and research workloads.

4. **BigQuery** – A scalable data analytics platform that can be used to analyze large datasets used in AI and machine learning projects.

---

## Client D – Global E-Commerce Company

**Scenario:** Multinational online shopping company, needs highly available infrastructure with automatic scaling.

**Recommended Platform:** AWS

**Justification:**

AWS is a strong choice for a global e-commerce company because it provides extensive global infrastructure and services designed for highly available and scalable applications. Services such as Amazon EC2 Auto Scaling and Elastic Load Balancing can automatically adjust computing capacity and distribute application traffic as demand changes. Amazon CloudFront can improve the delivery of websites, images, videos, and other content to customers around the world through a global content delivery network. AWS also provides globally distributed database and storage options that can support large e-commerce workloads and help maintain availability during periods of high traffic, such as major sales events.

**Services they could use:**

1. **Amazon EC2 Auto Scaling** – Automatically adjusts the number of EC2 instances based on application demand.

2. **Elastic Load Balancing (ELB)** – Distributes incoming traffic across multiple servers and Availability Zones to improve application availability and reliability.

3. **Amazon CloudFront** – A content delivery network (CDN) that delivers web content and application data to users with lower latency.

4. **Amazon Aurora Global Database** – Provides a globally distributed relational database architecture designed for applications that require high availability and fast access across multiple geographic locations.

---

## Summary

| Client | Recommended Platform | Main Reason |
|---|---|---|
| **Client A – Startup Company** | AWS | Flexible pricing, scalability, and broad range of services |
| **Client B – University** | Microsoft Azure | Strong integration with Microsoft 365, Windows Server, and Microsoft Entra ID |
| **Client C – AI Research Company** | Google Cloud Platform | Strong AI/ML infrastructure, GPUs/TPUs, Vertex AI, and Kubernetes |
| **Client D – Global E-Commerce Company** | AWS | Global infrastructure, scalability, load balancing, and CDN capabilities |


## Checkpoint 6 – Multi-Cloud Decision Matrix

| Business Requirement | Recommended Platform | Justification |
|---|---|---|
| Startup Company | **AWS** | AWS offers flexible pay-as-you-go pricing, a broad range of services, and scalable infrastructure that can support a startup as it grows. |
| Enterprise Organization | **AWS** | AWS provides extensive global infrastructure, mature enterprise support options, and a broad range of services and compliance programs suitable for large-scale operations. |
| Microsoft Environment | **Microsoft Azure** | Azure provides strong native integration with Microsoft Entra ID, Microsoft 365, Windows Server, SQL Server, and other Microsoft technologies, which can reduce migration and management complexity. |
| AI / Machine Learning | **Google Cloud Platform (GCP)** | GCP provides specialized AI and machine learning services, including Vertex AI and access to Google-designed Tensor Processing Units (TPUs), making it a strong choice for ML-focused workloads. |
| Kubernetes Deployment | **Google Cloud Platform (GCP)** | Google originally developed Kubernetes, and Google Kubernetes Engine (GKE) provides a mature managed Kubernetes platform with strong integration with Google Cloud services. |
| Global Web Application | **AWS** | AWS provides extensive global infrastructure, Amazon CloudFront for content delivery, and scalable compute and database services that can support applications serving users around the world. |

