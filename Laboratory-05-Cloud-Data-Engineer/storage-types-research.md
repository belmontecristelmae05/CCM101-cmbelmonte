# Storage Types Research

## Storage Comparison

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-size blocks and works like a disk attached to a computer or virtual machine. | Operating systems, databases, and applications | AWS EBS |
| File Storage | Stores data as files organized in folders and directories. | Shared files, documents, and applications that need a file system | AWS EFS |
| Object Storage | Stores data as objects with their data, metadata, and a unique identifier. | Photos, videos, backups, and other unstructured data | Amazon S3 |

## Why Object Storage is Suitable for User-Uploaded Images

Object storage is suitable for user-uploaded images because images are unstructured files that can be stored as individual objects. It can handle large amounts of data and allows applications to store and retrieve files using unique object identifiers. This makes it useful for applications that may receive many user-uploaded photos.
