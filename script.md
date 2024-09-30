[Java scripting](https://docs.oracle.com/en/java/javase/17/docs/api/java.scripting/javax/script/package-summary.html) allows to use script languages such as Groovy from Java and also make Java objects available to scripts.
Script languages are interpreted and you can bind decisions faster.

[Groovy](https://groovy-lang.org/) is especially great because its syntax is close to Java, it can use Java annotations, 
and once the logic is solidified Groovy can be compiled to Java class - you wouldn't need to re-write Groovy code in Java.
You can also create [Domain Specific Languages](https://docs.groovy-lang.org/docs/latest/html/documentation/core-domain-specific-languages.html) (DSLs) with Groovy.

It opens an opportunity to Domain-Specific Notations with possibly multiple DSLs for different types of diagram elements (processors).
E.g. business logic processors may use one DSL and back-end connectivity processors use another.

