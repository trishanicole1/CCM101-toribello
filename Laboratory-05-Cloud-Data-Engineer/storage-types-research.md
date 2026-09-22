# Storage Types Research

## Comparison Table

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|--------------|-------------|------------------|------------------------|
| Block Storage | Stores data in fixed-size blocks, with each block having its own address. It works like a virtual hard drive that can be attached to a server or virtual machine. | Databases, operating system boot volumes, and applications that require fast and low-latency read/write operations. | AWS EBS |
| File Storage | Organizes data using a traditional hierarchical structure of folders and files. It can be accessed by multiple systems through network protocols such as NFS or SMB. | Shared file systems, content management systems, and applications that require multiple servers to access the same files. | AWS EFS |
| Object Storage | Stores data as individual objects that contain the actual data, metadata, and a unique identifier. Objects are stored in a flat structure and are commonly accessed through HTTP-based APIs. | Large-scale storage of unstructured data such as photos, videos, documents, backups, and other media files. | AWS S3 |

## Why Object Storage is Best for Client Photos

Object Storage is the most suitable choice for a photo-sharing application that stores millions of user-uploaded images. Unlike Block Storage, it is not dependent on the physical storage capacity of a single server or virtual machine. It can scale to accommodate very large amounts of data.

Object Storage is also well suited for web and mobile applications because files can be uploaded, retrieved, and served through HTTP-based APIs. This makes it easy to integrate with modern application architectures.

Another advantage is that each stored object has a unique key and can contain metadata. This makes photos easier to organize, identify, retrieve, and manage. Object Storage is therefore a practical solution for applications that need reliable, scalable, and cost-effective storage for large collections of images.
