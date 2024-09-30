Below is the [URI syntax](https://medium.com/r/?url=https%3A%2F%2Fen.wikipedia.org%2Fwiki%2FUniform_Resource_Identifier%23syntax):

```
URI = scheme ":" ["//" authority] path ["?" query] ["#" fragment]
```

and [Data URL](https://medium.com/r/?url=https%3A%2F%2Fdeveloper.mozilla.org%2Fen-US%2Fdocs%2FWeb%2FURI%2FSchemes%2Fdata) syntax:

```
data:[<mediatype>][;base64],<data>["#" fragment]
```

There are the following variation points:

* Path
* Fragment
* Query - applicable to "remote" URIs

For example, a diagram author may use a library shape with pre-configured placeholder URIs in properties and customize path, fragment and query string, including using property placeholders (``%<property name>%``).
Similarly, an author of YAML specification may customize URIs used in bindings and use system properties and environment variables expansion tokens (``${<system property>}`` and ``${env.<environment variable>}``)
In Java and scripts developers may customize fragments and queries of URIs used to create invocables.

Script and spec remote URIs allow to implement distributed processing - script or spec source is generated on the server side parameterized by the query parameters and then executed on the client side parameterized by by the fragment.