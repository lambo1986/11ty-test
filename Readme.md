#### This is my first 11ty project, just as an experiment and learning tool. - Nathan Lambertson
#### Here are some steps I followed to set up the repo: 

# Setup Instructions

### Prerequisites

- **Node.js and npm**: Ensure you have Node.js and npm installed on your machine. You can install them using Homebrew:

  ```sh
  brew install node
  ```

- **Create a new project directory:**

  ```sh
  mkdir 11ty-test
  cd 11ty-test
  ```

- **Initialize a new npm project:**

  ```sh
  npm init -y
  ```

- **Install 11ty:**

  ```sh
  npm install --save-dev @11ty/eleventy
  ```

- **Create a basic directory structure:**

  ```sh
  mkdir src
  touch src/index.md
  ```

- **Add some content to src/index.md:**

  ```
  # Hello, 11ty!

  This is my first 11ty project.
  ```

- **Create an 11ty configuration file:**

  ```sh
  touch .eleventy.js
  ```

- **Add a basic configuration to .eleventy.js:**

  ```js
  module.exports = function(eleventyConfig) {
    return {
      dir: {
        input: "src",
        output: "dist"
      }
    };
  };
  ```

- **Update package.json to include build and serve scripts:**

  ```json
  {
    "name": "11ty-test",
    "version": "1.0.0",
    "description": "",
    "main": "index.js",
    "scripts": {
      "build": "eleventy",
      "serve": "eleventy --serve"
    },
    "keywords": [],
    "author": "",
    "license": "ISC",
    "devDependencies": {
      "@11ty/eleventy": "^1.0.0"
    }
  }
  ```

# Build and Serve the Project

- **Build the project:**

  ```sh
  npm run build
  ```
- **Serve the project locally:**

  ```sh
  npm run serve
  ```

- **Open your project in the browser:**
- Go to http://localhost:8080 to see your 11ty site.