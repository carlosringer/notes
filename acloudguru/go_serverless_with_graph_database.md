# Go Serverless with a Graph Database

## AWS Neptune

- good at handling complex data structures
- fully managageed graph database
- auto scaling handled by cloud formation
- uses familiar AWS services

Graph Models

- supports two types of graph modesl
- stored and queried seperately with their own query language
- Labeled Property Gprah and RDF (Resource Description Framework)
- RDF
  - SPARQL language
  - W3C web standard
- Property Graph
  - Gremlin QUery Language (Apache)
  - lead to development of neo4j
  - used in the course labs

Property Graph

- data is stored as vertices or nodes
- nodes connect to each other by edges (relationships)
  - edges can have properties
- edges and noeds have a defined type

Resouce Description Framework (RDF) Graph Model

- 2001 the idea of the semnatic web
  - RDF data would be a standard
  - would provide meta data for websites
  - powerful queries could be created based on RDF data, linking meaningful website data together
- like property graphs uses idea of nodes and edges
- no properties attached to edges
