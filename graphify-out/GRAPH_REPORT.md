# Graph Report - libra-domus-codicis  (2026-11-23)

## Corpus Check
- cluster-only mode — file stats not available

## Summary
- 98 nodes · 134 edges · 19 communities (7 shown, 12 thin omitted)
- Extraction: 98% EXTRACTED · 2% INFERRED · 0% AMBIGUOUS · INFERRED: 3 edges (avg confidence: 0.85)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `f4eceaa5`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- Community 0
- Community 1
- Community 2
- Community 3
- Community 4
- Community 5
- Community 6
- Community 7
- Community 8
- Community 9
- Community 10
- Community 11
- Community 12
- Community 13
- Community 14
- Community 15
- Community 16
- Community 17
- Community 18

## God Nodes (most connected - your core abstractions)
1. `download_book()` - 10 edges
2. `loadBooks()` - 8 edges
3. `log()` - 8 edges
4. `main()` - 8 edges
5. `renderFolderContents()` - 6 edges
6. `warn()` - 6 edges
7. `buildTreeHTML()` - 5 edges
8. `loadExplorer()` - 5 edges
9. `renderFolderTree()` - 5 edges
10. `scrape_baixe_livros()` - 5 edges

## Surprising Connections (you probably didn't know these)
- `remove_duplicates_philosophy.sh script` --calls--> `generate_books_json.sh script`  [EXTRACTED]
  scripts/remove_duplicates_philosophy.sh → scripts/generate_books_json.sh

## Import Cycles
- None detected.

## Communities (19 total, 12 thin omitted)

### Community 0 - "Community 0"
Cohesion: 0.24
Nodes (12): animateCounter(), books, categories, extractCategories(), filteredBooks, initMatrix(), loadBooks(), renderBooks() (+4 more)

### Community 1 - "Community 1"
Cohesion: 0.14
Nodes (13): runs-on, steps, jobs, check-duplicates, name, branches, branches, name (+5 more)

### Community 2 - "Community 2"
Cohesion: 0.47
Nodes (12): download_book(), error(), log(), main(), scrape_baixe_livros(), scrape_gutenberg(), scrape_gutenberg_direct(), scrape_internet_archive() (+4 more)

### Community 3 - "Community 3"
Cohesion: 0.30
Nodes (10): allBooks, buildFolderStructure(), buildTreeHTML(), countBooksInFolder(), folderStructure, initMatrix(), loadExplorer(), renderFolderContents() (+2 more)

### Community 4 - "Community 4"
Cohesion: 0.43
Nodes (5): books, initMatrix(), loadBookDetails(), renderBookDetails(), renderRecommendations()

### Community 5 - "Community 5"
Cohesion: 0.47
Nodes (4): generate_books_json.sh script, extract_core_name(), normalize_name(), remove_duplicates_philosophy.sh script

### Community 6 - "Community 6"
Cohesion: 0.83
Nodes (3): download_from_archive(), search_philosophy(), download_philosophy_smart.sh script

## Knowledge Gaps
- **2 isolated node(s):** `BOOKS`, `BOOKS`
  These have ≤1 connection - possible missing edges. (Counts symbols only; 37 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **12 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What connects `BOOKS`, `BOOKS` to the rest of the system?**
  _2 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Community 1` be split into smaller, more focused modules?**
  _Cohesion score 0.14285714285714285 - nodes in this community are weakly interconnected._