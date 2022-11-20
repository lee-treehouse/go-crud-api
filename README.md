# go-crud-api

go crud API inspired by 11 projects in one free code camp tutorial https://www.youtube.com/watch?v=jFfo23yIWac

# flowchart from video (TBC - attempting to recreate with mermaid.js)

```mermaid
flowchart LR

    get_all_route-->get_movies_function-->d1-->e1
    get_by_id_route-->get_movie_function-->d2-->e2
    a3-->create_route-->create_movie_function-->d3-->e3
    update_route-->update_movie_function-->d4-->e4
    delete_route-->delete_movie_function-->d5-->e5

subgraph Start
direction TB
a2(DATABASE)-->a3(MOVIES SERVER)
LOCALHOST:8000
end

subgraph Routes
    get_all_route(GET ALL)
    get_by_id_route(GET BY ID)
    create_route(CREATE)
    update_route(UPDATE)
    delete_route(DELETE)
end

subgraph Functions
    get_movies_function(getMovies)
    get_movie_function(getMovie)
    create_movie_function(createMovie)
    update_movie_function(updateMovie)
    delete_movie_function(deleteMovie)
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
