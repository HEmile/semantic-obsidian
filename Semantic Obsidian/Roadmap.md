---
aliases: []
---

## Planned
### [[Typed links plugin]]
A plugin that helps with creating and maintaining typed links. 
- Inline typed links
- Properties on links
- Preview typed links using templates
- Autocomplete typed links

### Minor
- Preview movie files using thumbnails

## Help wanted
These are  features that are out of scope for me to work on, but would be very useful to have.

### Port semantic markdown convert to Javascript
Currently, the [[Neo4j Graph View Plugin]] relies on [[Python]] for handling the conversion of Markdown to [[Neo4j]]. This makes it much harder for people to install the plugin. It's also not needed, because [[Javascript]] has a Neo4j driver https://github.com/neo4j/neo4j-javascript-driver. 

### Automatically update markdown based on Neo4j changes
Neo4j also has some useful authoring tools to create relational data. It'd be very cool if vaults could also be edited using those tools. Currently, it only works one way, from the markdown to Neo4j. The other way around is kind of dangerous: We don't want any data loss!



--- 

- hasTopic [[Semantic Obsidian]], [[Neo4j Graph View Plugin]]
- author [[Emile van Krieken]]