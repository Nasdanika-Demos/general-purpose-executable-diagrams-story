It is possible to associate multiple aspects/behaviors with diagram elements using processors and use diagrams from Java and scripts either directly or abstracted by interfaces implemented by dynamic proxies. 
You may have processors to generate documentation for multiple audiences and environments, multiple flavors of code (e.g. client libraries for different languages), infrastructure, ...
You can also have aspects to use a diagram as a runtime artifact.

Diagram authors may use �physical� URIs for aspects (processors) or �logical� which are mapped to physical. 
E.g. you may have ``my-company://storage/large`` logical URI which would be mapped, for example, to a URI which provides logic to connect to an S3 Bucket in a cloud deployment and to a shared drive in an on-prem deployment.

Diagram authors may also use libraries of reusable diagram elements with pre-configured aspects/processors.

Similar to scripts, diagrams can be stored in a source repository. 
Drawio web application can load and save diagrams from/to a variety of sources including GitHub.
Also, similar to scripts, diagrams may be bundled into jars and published to a binary repository.

Diagrams may be hosted on Confluence to make it convenient to for diagrammers. 
[Download attachments API](https://developer.atlassian.com/cloud/confluence/rest/v1/api-group-content---attachments/#api-wiki-rest-api-content-id-child-attachment-attachmentid-download-get) can be used by the client process to retrieve diagrams from Confluence.
On-prem Confluence may have a different API.


Diagram authors may use diagram properties placeholders to customize URIs.
