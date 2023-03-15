# Entry point is the main function
 Ex: fn main () {
    
 }

# The binary's Rust doesnt need runtime, once compiled, just distribute it among computers

# To compile simple source files
 $ rustc file.rs

# To compile projects with dependencies, use cargo tool
# Cargo is manager of project, a tool's manager and task executor of admistrative rotines over your project

# Create a new project
 $ cargo new project_name

# Building
 $ cargo build

# Cargo.toml file
# Is a proejct configuration file
# Includes version, packages and dependencies from others libraries and frameworks
# Similar to package.json as Node.js