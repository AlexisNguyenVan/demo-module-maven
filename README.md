# Demo-Module-Maven
Test changementsqsdfq

This repository is a simple project demonstrating how to split a project into maven module.

## How to build every module without installing them to the local maven repository

```
> mvn package # with tests
> mvn package -DskipTests # without tests
```

## How to build every module and install them to the local maven repository

```
> mvn install # with tests
> mvn install -DskipTests # without tests
> mvn install --non-recursive # only install the parent
> mvn install --projects greeting-app # only package and install greeting-app (requires the parent pom and greeting-components in the local .m2 repository)
```

