# Language-Cards

![language-cards](https://user-images.githubusercontent.com/101884444/178757500-e555b28e-e40e-4961-8da6-f43e237c5efa.gif)

[:point_right: Click here to see on browser](https://kaplan-react-language-card.netlify.app/)
---

| **What's used in this app ?**                                                | **How use third party libraries**          | **Author**                                                                       |
| ---------------------------------------------------------------------------- | ------------------------------------------ | -------------------------------------------------------------------------------- |
|  [useState() Hook](https://react.dev/learn#using-hooks)|                                            | [Take a look at my portfolio](https://kaplanh.github.io/Portfolio_with_CssFlex/) |
|  [Conditional rendering](https://react.dev/learn#conditional-rendering)   |                                  | [Visit me on Linkedin](https://www.linkedin.com/in/kaplan-h/)                    |
|  [rendering list](https://react.dev/learn#rendering-lists)                                                       |                                            |                                                                                  |
| [React-Bootstrap](https://react-bootstrap.netlify.app/)                      | npm i / yarn add react-bootstrap bootstrap |                                                                                  |
| Deploy with [Vercel](https://vercel.com/dashboard)                           |                                            |                                                                                  |

---

## How To Run This Project 🚀

<br/>

### 💻 Install React 👇

```bash
yarn create react-app .  or npx create-react-app .
```

### 💻 Install Sass 👇

```bash
yarn add sass  or npm i sass
```

## 🔴 Delete these files and delete the imports👇

    - App.test.js
    - reportWebVitals.js
    - setupTests.js
    - favicon.ico
    - logo192.png
    - logo512.png
    - manifest.json
    - robots.txt

### 💻 Start the project 👇

```bash
yarn start or npm start
```

OR

-   <strong>Clone the Repo</strong>

    ```sh
    git clone
    ```

-   <strong>Install NPM packages</strong>

    ```sh
    npm install or yarn
    ```

-   <strong>Run the project</strong>

    ```sh
    npm start or yarn start
    ```

-   <strong>Open the project on your browser</strong>

    ```sh
    http://localhost:3000/
    ```

-   ### <strong>Enjoy! 🎉</strong>

---

## Project Skeleton

```
Language-Cards App(folder)
|
|----public (folder)
│     └── index.html
|----src (folder)
|    |--- components (folder)
|    |       |── header(folder)
│    │       |     ├── Header.jsx
│    │       |     ├── Header.css
│    │       |
|    |       |── item(folder)
│    │       |     ├── Item.jsx
│    │       |     ├── Item.css
│    │       |
|    |       |── card(folder)
│    │             ├── Card.jsx
│    │             ├── Card.css
│    │
|    |--- helper (folder)
|    |       |── data.js                         
|    |                             
|    |--- assets (folder)
|    |       |── images                        
|    |       
│    ├--- App.js
│    ├--- App.css
│    └--- index.js
│    └--- img(folder)
│
│
|--- .gitignore
|── package-lock.json
├── package.json
|── README.md
|── yarn.lock



```

---

### At the end of the project, the following topics are to be covered;


        ```

-   conditional rendering

    ```jsx
    import { useState } from 'react';
    import './Item.css';
    
    const Item = ({ card }) => {
      const [showLogo, setShowLogo] = useState(true);
    
      const { name, img, options } = card;
    
      const handleClick = () => {
        setShowLogo(!showLogo);
      };
    
      return (
        <div className="card" onClick={handleClick}>
          {showLogo ? (
            <div>
              <img className="card-logo" src={img} alt="" />
              <h3 className="card-title">{name}</h3>
            </div>
          ) : (
            <ul className="list">
              {options.map((element, index) => {
                return <li key={index}>{element}</li>;
              })}
            </ul>
          )}
        </div>
      );
    };
    
    export default Item;
    ```

-   Rendiring list

    ```jsx
       <ul className="list">
          {options.map((element, index) => {
            return <li key={index}>{element}</li>;
          })}
        </ul>
    ```


---

## Feedback and Collaboration

I value your feedback and suggestions. If you have any comments, questions, or ideas for improvement regarding this project or any of my other projects, please don't hesitate to reach out.
I'm always open to collaboration and welcome the opportunity to work on exciting projects together.
Thank you for visiting my project. I hope you have a wonderful experience exploring it, and I look forward to connecting with you soon!

<p align="center"> ⌛<strong> Happy Coding </strong> ✍ </p>
