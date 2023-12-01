# Azure Storage

Azure Storage provides scalable and redundant solutions, ensuring data availability and durability. It supports automatic data replication across data centers for resilience against hardware failures or natural disasters. Additionally, security features include role-based access controls and encryption. The diverse range of services caters to specific application needs, offering flexibility for various  workloads and scenarios.

## Azure blob storage 
* Purpose: Designed for storing large amounts of unstructured data, such as images, videos, and documents.
* Features:
    *  Support block blobs, page blobs, and append blobs for different data access patterns.
* Usage Examples:
    * Storing images for a web application
    * Hosting videos for streaming services

* Designed for storage of files of any kind
    * Three storage tiers
        * Hot - frequently accessed data
        * Col - infrequently accessed data (lower availability, high durability)
        * Archive - rarely (if-ever) accessed data
	

## Azure Queue storage
* Purpose: provides message queues for asynchronous communication between application components, enabling the creation of distributed and resilient systems.
* Features:
    * Supports lightweight message operations like insert, read, and delete.
* Usage example:
    * Decoupling components in a microservices architecture.
    * Managing background tasks in a scalable application.
* Storage for small pieces of data (messages)
* Designed for scalable asynchronous processing

## Azure Table storage
* Purpose: offers schema-less key/value storage, ideal for large amounts of non-relational data, such as sensor or event logs.
* Features:
    * Automatic scalability, efficient indexing, and low-latency access.
* Usage examples:
    * Storing IoT device telemetry data.
    * Recording event logs in a distributed system.
* Storage for semi-structured data (NoSQL)
* No need for foreign joins, foreign keys, relationships or strict schema
* Designed for fast access
* Many programming interfaces and SDKs

## Azure File Storage
* Purpose: provides cloud-based shared storage, similar to traditional files systems, enabling multiple machines to access the same data concurrently
* Features:
    * Suitable for applications requiring shared access to files across multiple instances
* Usage Examples:
    * Shared configuration files among virtual machine instances.
    * Collaborative document editing with multiple users
* Storage for files accessed via shared drive protocols
* Designed to extend on-premise file shares or implement  lift-and-shift scenarios

## Azure Storage Account
* Group of services which include
    * Blob 
    * Queue
    * Table
    * File
* Used to store
    * Files
    * Messages
    * Semi-structured data
* Highly scalable (up to petabytes of data)
* Highly durable (99,9999999% - 11 nines, up to 16 nines)
* Cheapest per GB storage

* Azure Disk Storage
* Purpose: offers managed disks for azure virtual machines, providing persistent storage for operating system and application data.
* Features:
    * Disks can be used for individual virtual machines or grouped for shared storage.
* UsageExamples:
    * Storing application data on disks for a virtual machine
    * Configuring shared storage for a clustered application
* Disk emulation in the cloud 
* Persistent storage for Virtual Machines
* Different
    * sizes
    * types (SSD, HDD)
    * Performance tiers
* Disk can be un-managed or managed 

## Summary
* **Azure Storage Account** - Highly scalable and highly durable storage service consisting group of smaller services (blob, file, queue and table storage, fits any scenario)
* **Azure Blob Storage** - General purpose (blob) file storage, fits any scenario
* **Azure File Storage**  - File share service in the cloud, lift-and-shift scenarios
* **Azure Queue Storage**  - Service for storing small messages for asynchronous processing
* **Azure Table Storage** - Scalable NoSQL storage service for semi-structured data
* **Azure Disk Storage** - Disk emulation service in the cloud 