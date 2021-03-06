# Endpoints:

01. POST      {endpoint-url}/v1/game/new
02. PATCH     {endpoint-url}/v1/game/{id}/flag/{x}/{y}  (flag -> question mark -> unflag)
03. PATCH     {endpoint-url}/v1/game/{id}/reveal/{x}/{y}
04. POST      {endpoint-url}/v1/game/{id}/save
05. GET       {endpoint-url}/v1/game/{id}/resume

# Endpoints Response:

{
    "response": {
        face: "happy" | "sad",
        board: array[][]
    }
}

# To Consider

01. This endpoint should also recieve the level of the game or the custom parameters

