Because Microsoft built Dynamics 365 and Power Platform on Azure, customers are getting the same state-of-the-art security, privacy, and compliance protection used by 95 percent of Fortune 500 companies.

Microsoft Azure hosts Dynamics 365 business applications, and security is integrated into every aspect of it. Azure offers you unique security advantages derived from global security intelligence, sophisticated customer-facing controls, and a secure hardened infrastructure. This powerful combination protects your applications and data, supports your compliance efforts, and provides cost-effective security for organizations of all sizes.

This advantage is important for Microsoft because it's difficult for individual customers to achieve that same level of security internally.

#### Data ownership

You own your data, even when it’s located in a datacenter. Microsoft will use your and your customer’s data to provide only the services agreed upon, and for purposes that are compatible with providing those services. Microsoft doesn't share your data with advertiser-supported services, nor does it mine it for marketing or advertising. If you leave the service, Microsoft takes the necessary steps to ensure the continued ownership of your data. In other words, your data is secured in transit between user devices and the Microsoft datacenters.

#### Datacenter access

Cloud security starts with the physical security of the datacenters. Microsoft has an entire division devoted to designing, building, and operating the physical facilities that support Azure and the apps.

Dynamics 365 and Power Platform use a multiple layer approach to securing the use of applications and their data. Using a layered approach to physical security includes protecting the facility perimeter and building entrances—inside the building and the datacenter floor.

Customers using Dynamics 365 can take advantage of these security layers to implement their own governance of data and services.

### Introduction to cloud security

Microsoft implements security for Dynamics 365 based on customer requests, spanning from a simple security model with broad access all the way to highly complex security models, where each user is limited to specific record and field level access. Having a flexible application security model allows you to configure Dynamics 365 and Power Platform to meet even the most challenging business security models.

Microsoft Dataverse, the underlying data platform for Power Apps, handles the security—from user authentication to authorization—that allows users to perform actions with data and services.

Dynamics 365 and the Power Platform use a multiple layer approach to securing use of applications and their data. The following list is a high-level look at how the multiple layers of security that makes up the security model in Dataverse:

- Licensing is the first control-gate to allowing access to application components.
- Users are authenticated by Azure Active Directory (Azure AD). It can restrict access by users using conditional access policies.
- A user’s ability to see and use application resources is controlled by sharing the application with the user. Sharing of Power Apps is done directly with Dataverse security roles, while other applications can be shared with a user or Azure AD group.
- Environments act as security boundaries, allowing different security needs to be implemented in each environment.
- Environments with Dataverse add support for more advanced security models that are specific to controlling access to data.
- Connecter use can be further restricted with Data Loss Prevention (DLP) policies. Cross-tenant inbound and outbound restrictions can also be established.
- Ability to create a Power App and take advantage of Microsoft Power Automate is controlled by security roles in the context of environments.
- Power Automate and Power Apps use connectors. The specific connections credentials and associated service entitlements determine permissions when apps use the connectors.
- Ability to create applications and workflow is controlled by security roles in the context of environments.

Customers using Dynamics 365 can take advantage of these security layers to implement their own governance of data and services.

In addition to the configurable security controls, the platform also supports logging and auditing of data changes. Customers can view the logging in the Microsoft Compliance center. If customers use a Security Information and Event Management (SIEM) server, they can integrate the logging with their existing server.

An enterprise business solution must have a built-in security system that helps protect the database and its information from unauthorized access. The security system must also allow customers to specify what authorized users are allowed to do in the database and what data they can read and modify.

Now let's review some of the core concepts of cloud security, starting with encryption.
