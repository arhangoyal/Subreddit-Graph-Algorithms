# Subreddit-Graph-Algorithms

## CS225 Final Project

### Team
1. Arhan Goyal (arhang2)
2. Alex Ji (alexji2)
3. Amitabh Mahapatra (amitabh3)
4. Sara Alabbadi (saraa6)

---
## Project Files and Deliverables

### All Programs are in [code_base](code_base)
- [code_base/airport.h](code_base/airport.h) and [code_base/airport.cpp](code_base/airport.cpp)
- [code_base/page_rank.cpp](code_base/page_rank.cpp) and [code_base/page_rank.h](code_base/page_rank.h)
- [code_base/dijkstra.h](code_base/dijkstra.h) and [code_base/dijkstra.cpp](code_base/dijkstra.cpp)
- [code_base/heap.h](code_base/heap.h) and [code_base/heap.cpp](code_base/heap.cpp)
- [code_base/utils.h](code_base/utils.h) and [code_base/utils.cpp](code_base/utils.cpp)
- [code_base/main.h](code_base/main.h) and [code_base/main.cpp](code_base/main.cpp)

### Tests
- code_base/tests

### Data
- code_base/data/routes.csv
    - raw csv data from [OpenFlights](https://openflights.org/data.html)
- code_base/data/compressed.txt
    - compressed format generated by program

### Report
- [/0Documents/results.md](/0Documents/results.md)

### Video Presentation
- To be uploaded

---
## How to Run the Project Files?

## With Default Data
1. Pull the latest version of the project from our GitHub repository
2. Move into code_base directory using `cd code_base` and run `make`
2. Run `./main -csv` to generate compressed airport data
3. Run:

| Command                     | Description                                                                    | Example               |
| --------------------------- | ------------------------------------------------------------------------------ | --------------------- |
| `./main <any argument>`     | Invalid command. Lists available valid commands.                               | `./main`              |
| `./main -csv <file=default>`| Converts provided csv into compressed.txt. Default = `./data/routes.csv`       | `./main -csv`         |
| `./main -dk <src> <dest>`   | Dijkstra's Algorithm: Returns shortest weighted path and path length from `src` to `dest` airports.        | `./main -dk ORD DXB`  |
| `./main -pr <T/F>`          | Page Rank Algorithm: Returns 5 most or 1 least central airport(s), with parameter `T` or `F` respectively. | `./main -pr T`        |
| `./main -dfs <src> <dest>`  | Depth-First Search: Returns unweighted path from `src` to `dest` airports.     | `./main -bfs ORD DXB` |

### With Custom Data
1. Pull the latest version of the project from our GitHub repository
2. Move into code_base directory using `cd code_base` and run `make`
2. Run `./main -csv <filepath>` to generate compressed airport data
3. Run the available commands

### Run the Tests
1. Pull the latest version of the project from our GitHub repository
2. Move into code_base directory using `cd code_base` and run `make test`
3. Run `./test` (test are in ./code_base/tests)

---
## Tests included

### - General (not directly related to one algorithm)
   - readInCSV base case
   - readInCSV small scale test (large scale is too difficult to test)
   - Weighted Adjacency Matrix construction small test
   - Weighted Adjacency Matrix construction medium test (large scale is too difficult to test)
