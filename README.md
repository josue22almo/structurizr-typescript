# Structurizr for TypeScript

This GitHub repository is a port of [Structurizr for .NET](https://github.com/structurizr/dotnet) to TypeScript, in order to help you visualise, document and explore the software architecture of a software system. In summary, it allows you to create a software architecture model based upon Simon Brown's [C4 model](https://structurizr.com/help/c4).

[![npm version](https://badge.fury.io/js/structurizr-typescript.svg)](https://www.npmjs.com/package/structurizr-typescript)

[![Actions Status](https://github.com/ChristianEder/structurizr-typescript/workflows/npm%20publish/badge.svg)](https://github.com/ChristianEder/structurizr-typescript/actions)

## How to use

- Set up a new project similar to this [sample](https://github.com/ChristianEder/structurizr-typescript/tree/master/sample)
  > npm init\
  > npm install -D @types/node\
  > npm install -D typescript\
  > npm install -S structurizr-typescript
- Start coding your architecture model similar to the [sample index.ts](https://github.com/ChristianEder/structurizr-typescript/blob/master/sample/index.ts)
  - For more detailed documentation on how to use Structurizr, please refer to [Structurizr for .NET](https://github.com/structurizr/dotnet) - the usage is pretty much the same
  - In the current version of this package, not all of Structurizrs features are already implemented. See [Limitations](#Limitations) section below

## Limitations

The current version of this package supports:
- Person, SoftwareSystem, Container, Component & CodeElement entities
- Relationships between those entities 
- System Context, Container & Component diagrams
- Deployment diagrams with DeploymentNode, ContainerInstance and HttpHealthCheck entities
- Filtered Views
- Custom Element & Relationship styles, usage & export of themes
- Documentation Sections & Decisions (kudos go to [Joe Ruello](https://github.com/joeruello))
- Diagram Autolayouting (kudos go to [Joe Ruello](https://github.com/joeruello))
- Diagram paper size settings
- Custom Branding & Terminology

This specifically excludes:
- Encrypted workspaces
- Dynamic diagrams 
- Enterprise context diagrams

Also, as of now the package has just a few automated tests - use at own risk :-). Let me know if you encounter any issues, I am happy to provide a fix.
