# SiteKit  

SiteKit is a command-line tool designed to simplify the creation, building, and serving of static websites. It provides a streamlined workflow for developers to quickly scaffold new projects, build static assets, and serve them locally for testing.  

## Features  
- **Project Scaffolding**: Quickly create a new site project using predefined templates.  
- **Static Site Building**: Build static assets from source files, including HTML and Markdown.  
- **Local Development Server**: Serve your site locally for testing and development.  
- **Customizable Templates**: Use or create templates to standardize your site structure.  

## Requirements  
- .NET 8.0 or later  
- Basic knowledge of command-line tools  

## Installation  

1. Clone the repository or download the source code.  
2. Build the project using the .NET CLI:
3. Install the tool globally:
```bash
git clone https://github.com/CodingBoson/SiteKit.git
cd ./SiteKit

./install.ps1 # For Windows
./install.sh # For Linux/MacOS
```
## Usage  

### Commands  

#### `new`  
Create a new site project.
- `siteName`: The name of the new site project.  
- `-t, --template`: (Optional) The template to use. Defaults to `default`.  

#### `build`  
Build the static site from source files.
#### `serve`  
Serve the site locally for testing.
- `-u, --url`: (Optional) The URL to serve the site. Defaults to `http://localhost:9443/`.  
- `-u, --url`: (Optional) The URL to serve the site. Defaults to `http://localhost:9443/`.  
- `--no-build`: (Optional) Skip the build step before serving.  

## Project Structure  

A typical SiteKit project has the following structure:
```bash
myBlog/
├─ Pages/          # Your Markdown or HTML pages
├─ wwwroot/        # CSS, images, JS, etc.
├─ sitekit.json    # Site configuration (title, properties, etc.)
└─ publish/        # Auto-generated static output
```

## Configuration  

The `sitekit.json` file contains the configuration for your site. Example:
```json
{
  "Name": "SiteKit",
  "Properties": {}
}
```

## Development  

### Building the Project  

To build the project, run:
~~~bash
sitekit build
~~~
### Running Tests  

To run the tests, use:
~~~bash
sitekit serve
~~~
