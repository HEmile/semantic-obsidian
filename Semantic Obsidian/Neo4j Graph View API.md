---
aliases: [API]
---

![[Roadmap#^82c7c4]]

## Requirements
Users of the API should be able to extend the Neo4j Graph View in the following ways. If something is missing, please [[Discord|let me know.]]

### Add additional data
Add additional nodes and relations to the graph. This could for instance be used to [connect papers to their citations](https://forum.obsidian.md/t/show-online-literature-connections/10924) (and to papers they cite), like in [Connected Papers](https://www.connectedpapers.com/). There are many other sources of information to extract data from.

Other ideas might be extracting a graph from the Markdown, such as adding the outline of a note like in the [Mind Map plugin](https://github.com/lynchjames/obsidian-mind-map), or developing new syntax for generating graphs. 

### Manipulate the Graph View
Add UI's on top of the graph view, or add ways of interacting with the visualization. Expose functionality in the NeoVisView. 
Possible hooks:
- Initialization of the visualization
	- Allows hooking into the vis.js network.
- Context menu
- Before query
- After nodes are added

### Manipulate styling of the graph
Allow plugins to manipulate the styling of [[Node styling|nodes]] and [[Edge styling|edges]]. 

### Query the Neo4j data
Plugins should be able to query the [[Neo4j]] database to allow reusing the graph-based format and quick, easy querying with [[Cypher]]. 

--- 
#development 
- hasTopic [[Neo4j Graph View Plugin]]
- author [[Emile van Krieken]]