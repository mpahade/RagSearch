# RagSearch

A search page for course handouts stored in Neo4j. Type a query and the page shows matching passages, with your search words highlighted.

The page sends each search to an n8n webhook, which queries the Neo4j graph (`(:Document)-[:HAS_CHUNK]->(:Chunk)`) and returns the best-matching passages. No database credentials are stored in this repository.

Hosted with GitHub Pages.
