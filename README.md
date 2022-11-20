# go-crud-api

go crud API inspired by 11 projects in one free code camp tutorial https://www.youtube.com/watch?v=jFfo23yIWac

# flowchart from video (TBC - attempting to recreate with mermaid.js)

```mermaid
flowchart LR

    b1-->c1-->d1-->e1
    b2-->c2-->d2-->e2
    a3-->b3-->c3-->d3-->e3
    b4-->c4-->d4-->e4
    b5-->c5-->d5-->e5


subgraph Start
direction TB
a2(DATABASE)-->a3(MOVIES SERVER)
LOCALHOST:8000
end


    subgraph Routes
b1(GET ALL)
b2(GET BY ID)
b3(CREATE)
b4(UPDATE)
b5(DELETE)
    end

subgraph Functions
c1(getMovies)
c2(getMovie)
c3(createMovie)
c4(updateMovie)
c5(deleteMovie)
    end

subgraph Endpoints
d1("/movies")
d2("/movies/id")
d3("/movies")
d4("/movies/id")
d5("/movies/id")
    end

subgraph Methods
e1(GET)
e2(GET)
e3(POST)
e4(PUT)
e5(DELETE)
    end


```
