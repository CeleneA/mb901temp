You own your data and Microsoft protects it with encryption. Connections established between customers and Microsoft datacenters are encrypted, and all public endpoints are secured using industry-standard Transport Layer Security (TLS). TLS establishes a security-enhanced browser to server connection to ensure data confidentiality and integrity between desktops and datacenters. TLS also protects API access from the customer endpoint to the server.

Model-driven apps in Dynamics 365 use standard SQL Server cell-level encryption for a set of default entity attributes that contain sensitive information, such as usernames and email passwords. This feature can help organizations achieve FIPS 140-2 compliance.

> [!NOTE]
> Although FIPS 140-2 is a U.S./Canadian Federal standard, FIPS 140-2 compliance has been widely adopted around the world in both governmental and non-governmental sectors as a practical security benchmark and realistic best practice.
### Encryption at rest

All instances of the Microsoft Dataverse database use SQL Server Transparent Data Encryption (TDE) to perform real-time encryption of data when written to disk, also known as encryption at rest. 

Encryption at rest prevents attackers from accessing the unencrypted data by ensuring the data is encrypted when on disk. If an attacker obtains a hard drive with encrypted data but not the encryption keys, the attacker must defeat the encryption to read the data. This attack is much more complex and resource consuming than accessing unencrypted data on a hard drive. For this reason, encryption at rest is highly recommended and is a high priority requirement for organizations.

### Encryption keys

By default, Microsoft stores and manages the database encryption keys for Dataverse instances, so you don’t have to. 

The *manage keys* feature—in the Dynamics 365 Administration Center—gives administrators the ability to self-manage the database encryption keys that are associated with instances of Dynamics 365 (online). Microsoft recommends that we manage the keys, unless you have a specific business need to maintain your own.

You create encryption keys using algorithms designed to make sure that each key is unique and unpredictable. The .NET Framework Data Protection API generates the keys used by Dynamics 365 business applications. Each tenant supports having a single encryption key. To use the encryption methods, you must create a key.

Now let's review authentication.
