<div id="top"></div>

<!-- PROJECT LOGO -->
<br />
<div align="center">
<h3 align="center">React VSCode Themed Portfolio</h3>

  <p align="center">
    <a href="https://mint13.github.io/">Demo</a>
    ·
    <a href="https://mint13.github.io/#/docs">Markdown Preview</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>        
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#demonstration">Demonstration</a></li> 
    <li><a href="#features">Features</a></li>        
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project


The project is inspired by [Visual Studio Code](https://github.com/microsoft/vscode) and [caglarturali.github.io](https://github.com/caglarturali/caglarturali.github.io). The pages of the portfolio are powered by `markdown`, which make them easy to modify or add your own contents.

<p align="right">(<a href="#top">back to top</a>)</p>

### Built With

* [React.js](https://reactjs.org/)
* [Material UI](https://github.com/mui/material-ui)
* [react-markdown](https://github.com/remarkjs/react-markdown)

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- GETTING STARTED -->
## Getting Started

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/mint13/mint13.github.io.git
   ```
2. Install NPM packages
   ```sh
   npm install
   ```
3. Enter your name in `.env.development`
   ```js
   REACT_APP_NAME=<your_name>
   ```
4. Add your markdown pages in `public/pages`
5. Add your routes in `src/app/pages/page.ts`, make sure the names of pages are consistent with markdown files.
    ```ts
    export const pages = [
      { index: 0, name: 'overview.md', route: '/overview' },
      { index: 1, name: 'skills.md', route: '/skills' },
      { index: 2, name: 'experience.md', route: '/experience' },
      { index: 3, name: 'education.md', route: '/education' },
      { index: 4, name: 'projects.md', route: '/projects' },  
      { index: 5, name: 'certificates.md', route: '/certificates' },
      { index: 6, name: 'accomplishments.md', route: '/accomplishments' },
    ];
    ```
6. Add your social links in `src/app/pages/link.tsx`, which will appear in both sidebar and homepage.
    ```ts
    export const links = [
      {
        index: 0,
        title: "Find me on Github",
        href: "https://github.com/noworneverev",
        icon: <FaGithub />,
      },
    ];
    ```
7. Runs the app in the development mode
   ```sh
   npm start
   ```   
8. Deploy your own portfolio,  
   - modify homepage property in `package.json` 
   ```
   "homepage": "https://{username}.github.io/{repo-name}"
   ```
   > \* For a [project site](https://pages.github.com/#project-site), that's the format. For a [user site](https://pages.github.com/#user-site), the format is: `https://{username}.github.io`. You can read more about the `homepage` property in the ["GitHub Pages" section](https://create-react-app.dev/docs/deployment/#github-pages) of the `create-react-app` documentation.   
  


   - modify Google Analytic measurement id in `.env.production`
   ```
   REACT_APP_NAME=<your_name>
   REACT_APP_MEASUREMENT_ID=<your_measurement_id>   
   ```

### Alternative Deployment
```
docker-compose up
```

<p align="right">(<a href="#top">back to top</a>)</p>

## Demonstration

- The project is deployed to following two domains, and they are in synchronization.
  - user site: [https://mint13.github.io/](https://mint13.github.io/)
  - project site: [https://github.com/mint13/mint13.github.io](https://github.com/mint13/mint13.github.io)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Features

- Powered by markdown
- Extended markdown syntax supported
  - Syntax highlight
  - Alert
- Dark mode and light mode available
- Closable tabs
- Collapsible explorer
- Responsive web design
- Google Analytics supported
- Auto-deploy to gh-pages with github actions ready

Markdown preview: https://mint13.github.io/#/docs

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.md` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Yan-Ying Liao - [Personal Portfolio](https://mint13.github.io/) - n9102125@gmail.com

Project Link: [https://github.com/mint13/mint13.github.io](https://github.com/mint13/mint13.github.io)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [React Icons](https://react-icons.github.io/react-icons/search)
* [caglarturali.github.io](https://github.com/caglarturali/caglarturali.github.io)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[forks-shield]: https://img.shields.io/github/forks/noworneverev/react-vscode-portfolio
[forks-url]: https://github.com/mint13/mint13.github.io/network/members
[stars-shield]: https://img.shields.io/github/stars/noworneverev/react-vscode-portfolio
[stars-url]: https://github.com/mint13/mint13.github.io/stargazers
[issues-shield]: https://img.shields.io/github/issues/noworneverev/react-vscode-portfolio
[issues-url]: https://github.com/mint13/mint13.github.io/issues
[license-shield]: https://img.shields.io/github/license/noworneverev/react-vscode-portfolio
[license-url]: https://github.com/mint13/mint13.github.io/blob/master/LICENSE.md
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/yan-ying-liao/
[product-screenshot]: ./src/static/screenshot.gif
[gh-pages-shield]: https://img.shields.io/github/deployments/noworneverev/noworneverev.github.io/github-pages
[gh-pages-url]: https://github.com/noworneverev/noworneverev.github.io/deployments
[website-shield]:https://img.shields.io/website?url=https%3A%2F%2Fnoworneverev.github.io%2F
[website-url]: https://mint13.github.io/