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

### [[Neo4j Graph View API]]
After [[#Port semantic markdown convert to Javascript|porting to Javascript]], it should be possible to create an API for other plugin developers to use, to interact with the [[Neo4j Graph View Plugin]]. This could allow extending the graph view with eg automatically adding data from external sources (eg citation graphs), or with different syntax for creating graphs. ^82c7c4

### Graph View Filtering
Add a pane in the Graph View with which you can filter the graph by for example tags, folders or name. Help in designing this Graph View is very welcome. Join the [[Discord]] if you are good at UX design and want to help out.

### Save state of graph
Currently, the state of the graph cannot be saved, and will be lost once the pane closes (or upon Obsidian restart). It'd be very useful to save graphs to get back in this 'workspace'. 

### Node locking
Often, one would want to create a specific layout and then lock nodes in place so they don't randomly move around, losing oversight of the view. "Locking" nodes would put nodes in place, so one can remember where to look.


### Minor
- Preview movie files using thumbnails
- Add external (Markdown) links to the graph. Clicking on that node opens the link in your browser

## Help wanted
These are  features that are out of scope for me to work on, but would be very useful to have.

### Automatically update markdown based on Neo4j changes
Neo4j also has some useful authoring tools to create relational data. It'd be very cool if vaults could also be edited using those tools. Currently, it only works one way, from the markdown to Neo4j. The other way around is kind of dangerous: We don't want any data loss!

### Styling interface
Styling of [[Node styling|nodes]] and [[Edge styling|edges]] is currently done using plaintext in .json. This isn't very accessible, and a bit hard to use. It would be nice if there's a useful for interface for basic styling use, like in Neo4j Bloom.


--- 
#development
- hasTopic [[Semantic Obsidian]], [[Neo4j Graph View Plugin]]
- author [[Emile van Krieken]]