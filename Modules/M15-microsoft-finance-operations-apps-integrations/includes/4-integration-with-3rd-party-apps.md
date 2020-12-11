When deciding on an integration pattern and technology, it's important to first understand the business need and requirements. Then can you translate the need to the proper technology. For instance, is real-time integration possible or will you require batch-based integrations for the data volumes?

Finance and operations apps allow for several patterns of integrations.

### Open Data Protocol (OData)

OData is an open protocol. It allows the creation and consumption of queryable and interoperable RESTful APIs in a simple and standard way.

APIs specify the way you structure information passed across platforms so that applications can exchange data and information. Representational State Transfer (REST) is an API architectural style. A developer creates the API on the server and allows the client to talk to it. REST then decides what the API looks like.

OData allows the creation of REST-based web services. These services find resources using Uniform Resource Locators (URLs) and you define them in a data model. They publish and edit the web services by web clients using HTTP messages.

OData helps applications focus on business logic without worrying about the various API approaches to define request and response headers, status codes, payload formats, or query options. OData supplies guidance for tracking changes, defining functions or actions for reusable procedures, and sending asynchronous or batch requests.

> [!NOTE]
> OData has a limit of returning 10,000 records per call. To retrieve more data, you must implement pagination logic for integration scenarios.

We recommend that you use OData integration for low to medium volume data integration. It's an exceptional architecture choice for real-time integrations for small data sets.

### Custom webservices

Finance and Operations apps support the development of custom webservices. You always expose custom webservices via a SOAP and a JavaScript Object Notation (JSON) endpoint. JSON support is a new feature in Dynamics 365 Finance and allows for the return data set to be in JSON format. We recommend this integration for real-time integration needs for small to mid-size data sets.

### Data management package REST API

While OData works for small data sets, we recommend the data management package integration architecture for large data sets that don’t require real-time scheduling.

The package REST API lets you integrate by creating a request in Dynamics 365 Finance for a downloadable data package.

Now let's turn our attention to business events.
