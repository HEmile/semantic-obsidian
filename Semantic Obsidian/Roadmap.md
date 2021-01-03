---
aliases: []
---

## Next
### Port semantic markdown convert to Javascript
Currently, the [[Neo4j Graph View Plugin]] relies on [[Python]] for handling the conversion of Markdown to [[Neo4j]]. This makes it much harder for people to install the plugin. It's also not needed, because [[Javascript]] has a Neo4j driver https://github.com/neo4j/neo4j-javascript-driver. 
There is also a nice query builder which could be useful: https://github.com/jamesfer/cypher-query-builder

## Planned

### [[Link Types]]
Add better support for creating and maintaining link types. Also provide new syntax for inline link types and properties on links. A discussion on syntax is in [[Link Types]].
- Inline typed links
- Properties on links
- Preview typed links using templates
- Autocomplete typed links

### [[Semantic Obsidian API]]
After [[#Port semantic markdown convert to Javascript|porting to Javascript]], it should be possible to create an API for other plugin developers to use, to interact with the [[Neo4j Graph View Plugin]]. This could allow extending [[Semantic Obsidian]] with eg automatically adding data from external sources (eg citation graphs), or with different syntax for creating graphs.

### Graph View Filtering
Add a pane in the Graph View with which you can filter the graph by for example tags, folders or name. Help in designing this Graph View is very welcome. Join the [[Discord]] if you are good at UX design and want to help out.

### Minor
- Preview movie files using thumbnails

## Help wanted
These are  features that are out of scope for me to work on, but would be very useful to have.

### Automatically update markdown based on Neo4j changes
Neo4j also has some useful authoring tools to create relational data. It'd be very cool if vaults could also be edited using those tools. Currently, it only works one way, from the markdown to Neo4j. The other way around is kind of dangerous: We don't want any data loss!



--- 
#development
- hasTopic [[Semantic Obsidian]], [[Neo4j Graph View Plugin]]
- author [[Emile van Krieken]]