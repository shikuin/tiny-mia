tract-mia-axum

--- 
## REQUIREMENT FOR PROJECT

> Logger and initialization of model, server, packages (enviroment)
> Auto-setup model by installation
> TinyGPT-2 that procedes with tract.rs
> Small server in Axum that will output\input of model
> Auth setup (JWT token)
> Structure with two big crates (not in one)

--- 
## FOR THE FUTURE

> Rewrite in gRPC 
> Access to mia from no jwt, but another one
> Tooling for loader of model (orchestrator)

--- 
## TODOS (restructure todos based on REQUIREMENT FOR PROJECT) 

> Organize mia and server, tiny-mia folder
> Organize folders and files: From higher abstraction to Lower abstraction
> Make a logger
> Organize configuration: Where to store (container, auth)
> Write axum router
> Write handlers for JSON
> Write jwt-token for auth
> Add handler for contrainer to download TinyGPT-2 for tract
> Handle loading model
> Handle model generation and sending data

--- 
## STRUCTURE OF PROJECT

- main.rs -> setup, load and config

- server/ -> axum
- server/main.rs -> axum setup, initialization
- server/router.rs -> router of axum 
- server/handlers.rs -> handlers for JSON messages

- mia/main.rs -> initialization of model
- mia/tract.rs -> handle of loading model



