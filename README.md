# Finch Fashion Ecommerce Website
  -Live Site URL: [https://jul-lactao.netlify.app/](https://jul-lactao.netlify.app/)

  -Ecommerce website using Next.js as framework and Shoppify to handle the data for our products from our store and lastly using Builder.io for the frontend design.
  
## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My Process](#process)
  - [Errors](#errors)
  - [Built With](#built-with)
- [Author](#author)

## Overview

### Screenshot

![](./_readme_img/portfolio.png)

### Links

  -Live Site URL: [https://jul-lactao.netlify.app/](https://jul-lactao.netlify.app/)

## My Process
1.  **Setup the projects.**

    Set up the starter and follow the intructions ([install instructions](https://github.com/BuilderIO/nextjs-shopify))


1.  **Start developing.**

    Navigate into your new site’s directory and start it up.

    ```shell
    cd my-hello-world-starter/
    gatsby develop
    ```

1.  **Open the source code and start editing!**

    Your site is now running at `http://localhost:8000`!

    _Note: You'll also see a second link: _`http://localhost:8000/___graphql`_. This is a tool you can use to experiment with querying your data. Learn more about using this tool in the [Gatsby Tutorial](https://www.gatsbyjs.com/docs/tutorial/part-4/#use-graphiql-to-explore-the-data-layer-and-write-graphql-queries)._

    Open the `my-hello-world-starter` directory in your code editor of choice and edit `src/pages/index.js`. Save your changes and the browser will update in real time!


---

### Errors

1.  **Package path not exported**

    ```shell
    Error [ERR_PACKAGE_PATH_NOT_EXPORTED]: Package subpath './lib/tokenize' is not defined by "exports" in the package.json of a module in node_modules
    ```
    SOLUTION: Downgrade Node.js to version 17.4.0

    `([LINK:](https://stackoverflow.com/questions/69693907/error-err-package-path-not-exported-package-subpath-lib-tokenize-is-not-d))`

1.   **It Looks Like You're Trying To Use Typescript**

    ```shell
    Please install @types/react by running:

        npm install --save-dev @types/react

    If you are not trying to use TypeScript, please remove the tsconfig.json file from your package root (and any TypeScript files in your pages directory).
    ```

    SOLUTION: I ran the code attached to update some dependencies fixed at 17.0.0 but instead of solving the problem, another problem arise which is the third error below. So what I did, I revert the installation I made and put it back to its original version.
    ```shell
    npm install --save-dev typescript @types/react@17.0.0 @types/node@17.0.0 @types/react-dom@17.0.0
    ```

    `([LINK:](https://stackoverflow.com/questions/70106900/react-typescript-it-looks-like-youre-trying-to-use-typescript-but-do-not-have))`

1. **Digital envelope routines unsupported**

    ```shell
    node:internal/crypto/hash:67   this[kHandle] = new _Hash(algorithm, xofLen);                  
     ^  Error: error:0308010C:digital envelope routines::unsupported
    ```

    SOLUTION: Just follow the instructions from the link.
    `([LINK:](https://bobbyhadz.com/blog/react-error-digital-envelope-routines-unsupported))`

---

### Built with

- Semantic HTML5 markup
- Tailwind
- NextJS
- Builder.io

---
 
## Author

- Twitter - [@julfinch](https://www.twitter.com/julfinch)
