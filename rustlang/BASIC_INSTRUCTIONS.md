# Entry point is the main function
 Ex: fn main () {
    
 }

# The binary's Rust doesnt need runtime, once compiled, just distribute it among computers

# To compile simple source files
 $ rustc file.rs

# To compile projects with dependencies, use cargo tool
 - Cargo is manager of project, a tool's manager and task executor of admistrative rotines over your project

# -----------------Commands--------------------------
# Create a new project
 $ cargo new project_name

# Building
 $ cargo build

# Automating most of the previos commands
 $ cargo run

# Formatting code
 $ cargo fmt
# -----------------------------------------------------------
# Cargo.toml file
 - Is a project configuration file
 - Includes version, packages and dependencies from others libraries and frameworks
# Similar to package.json as Node.js


# Rust Workspace
 - Always when there is a Cargo.toml in a Project, that is a workspace for rustlang
 - Cargo.toml is necessary as well in order to building the project to gathering dependecies and so on.
 - The default proceduring to generate a binary is debug mode within the "Target" directory
 - To buid in production must include --release at the command cargo build

 # ------------------Tools ----------------------------------
 # Watching code
   $ cargo install cargo-watch
   $ cargo watch -x run
 # -----------------------------------------------------------
  