# Endpoints:

[DONE]
01. POST      {endpoint-url}/ms-api/games
02. PATCH     {endpoint-url}/ms-api/games/{id}/flag/{x}/{y}  (flag -> question mark -> unflag)
03. PATCH     {endpoint-url}/ms-api/games/{id}/reveal/{x}/{y}
06. GET       {endpoint-url}/ms-api/games
07. GET       {endpoint-url}/ms-api/games/{id}
08. PATCH     {endpoint-url}/ms-api/games/{id}      { name: "" }

[TODO]
04. POST      {endpoint-url}/ms-api/games/{id}/save
05. GET       {endpoint-url}/ms-api/games/{id}/resume

# Endpoints Response:

board: {
    id: string,
    size: int,
    numMines: int,
    happy: boolean,
    matrix: square[][]
}

square: {
    type: string: mine|number,
    value: int,
    opened: boolean,
    flag: string: flag|question|none,
    row: int,
    col: int
}

# To Consider

01. This endpoint should also recieve the level of the game or the custom parameters

# Issues

01. [DONE] This endpoint should response with a board autogenerated ID
03. [DONE] When a mine is found the board must only reveal all the mines
03. [DONE] When a mine is found the board should record the last mine revaled
01. 02. 03. The square in the response must only include the type and value after the squared has been revealed


# To Consider Globally
* [DONE] Add Swagger configuration for documenting the API
