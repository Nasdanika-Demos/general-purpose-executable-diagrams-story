YAML or JSON spec can be used to bind configuration decisions - variables/bindings, versions of dependencies. 
The spec may contain invocable URIs, so you may compose solutions from building blocks published as URIs.

In the future specs will support multiple inheritance as shown on the above diagram.
For example, you may have a generic dashboard prototype and a specialized dashboard for one of your clients/partners/LOBs - Acme Corporation.
Then you may have a hierarchy of POC/Lab environment configurations.
An executable spec of the dashboard prototype for Acme Corporation to run on Sandbox A would extend two specs.
Please note that this is not a new idea, more like an application of the old idea which does not require dedicated infrastructure - all of the above can be stored in a version control system like GitHub.

Specs also support value interpolation with Java system properties and environment variables.

Similar to scripts and diagrams, specifications can be stored to version control and published to binary repositories. They can also be encoded into data URLs similar to scripts.