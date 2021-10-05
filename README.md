# Microfront end Ecomm

## Lifecycle of ModuleFederationPlugin

1 It loads container index.js
2 Then it loads remoteEntry.js files of both sub projects
3 Followed by loading bootstrap file of container
4 It then loads src folders of sub projects and the shared lib files
5 Finally loads bootstrap files of sub projects

## Advantages of ModuleFederationPlugin

- Have shared library of files, between multiple projects
- Force shared library to be loaded once by using singleton true
- Async load scripts, before executing them

\*\* Singleton load doesn't load multiple major versions, instead it will throw out warning message only.
