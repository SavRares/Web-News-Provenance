<div align="center">

  <h1>Web News Provenance</h1>
  
  <p>
    The platform where you can get your news 
  </p>
  
  
<!-- Badges -->
<p>
  <a href="https://github.com/SavRares/Web-News-Provenance/graphs/contributors">
    <img src="https://img.shields.io/github/contributors/SavRares/Web-News-Provenance" alt="contributors" />
  </a>
  <a href="">
    <img src="https://img.shields.io/github/last-commit/SavRares/Web-News-Provenance" alt="last update" />
  </a>
  <a href="https://github.com/SavRares/Web-News-Provenance/network/members">
    <img src="https://img.shields.io/github/forks/SavRares/Web-News-Provenance" alt="forks" />
  </a>
  <a href="https://github.com/SavRares/Web-News-Provenance/stargazers">
    <img src="https://img.shields.io/github/stars/SavRares/Web-News-Provenance" alt="stars" />
  </a>
  <a href="https://github.com/SavRares/Web-News-Provenance/issues/">
    <img src="https://img.shields.io/github/issues/SavRares/Web-News-Provenance" alt="open issues" />
  </a>
  <a href="https://github.com/SavRares/Web-News-Provenance/blob/master/LICENSE">
    <img src="https://img.shields.io/github/license/SavRares/Web-News-Provenance.svg" alt="license" />
  </a>
</p>
   
<h4>
    <a href="https://github.com/SavRares/Web-News-Provenance/">View Demo</a>
  <span> · </span>
    <a href="https://github.com/SavRares/Web-News-Provenance">Documentation</a>
  <span> · </span>
    <a href="https://github.com/SavRares/Web-News-Provenance/issues/">Report Bug</a>
  <span> · </span>
    <a href="https://github.com/SavRares/Web-News-Provenance/issues/">Request Feature</a>
  </h4>
</div>

<br />

<!-- Table of Contents -->

# :notebook_with_decorative_cover: Table of Contents

- [About the Project](#star2-about-the-project)
  - [Screenshots](#camera-screenshots)
  - [Tech Stack](#space_invader-tech-stack)
  - [Features](#dart-features)
  - [Color Reference](#art-color-reference)
  - [Environment Variables](#key-environment-variables)
- [Getting Started](#toolbox-getting-started)
  - [Prerequisites](#bangbang-prerequisites)
  - [Run Locally](#running-run-locally)
  - [Deployment](#triangular_flag_on_post-deployment)
- [Roadmap](#compass-roadmap)
- [Contributing](#wave-contributing)
- [License](#warning-license)
- [Contact](#handshake-contact)

<!-- About the Project -->

## :star2: About the Project

<!-- Screenshots -->

### :camera: Screenshots

<div align="center"> 
  <p>Once you entered our platform a landing page will be loaded, where one can login/create an account.</p>
  <img src="./assets/landing-page.png" alt="landing page" />
  <p> When signing in the user will be redirected to another page to Sign-In trough our Identity provider, Clerk.</p>
  <img src="./assets/sing-in.png" alt="sign in page" />
  <p>Once authenticated the user will be able to scroll trough multiple news available on our platform, and of course read their details by clicking on the cards.</p>
  <img src="./assets//news-page.png" alt="news page" />
  <img src="./assets/news-details-page.png" alt="news details page"/>
  <p>Another page available for users is the "SPARQL Query" page where users can write SPARQL queries and receive answers in different formats</p>
  <img src="./assets//sparql-query-page.png" alt="sparql query page"/>
</div>

<!-- TechStack -->

### :space_invader: Tech Stack

<details>
  <summary>Client</summary>
  <ul>
    <li><a href="https://www.typescriptlang.org/">Typescript</a></li>
    <li><a href="https://nextjs.org/">Next.js</a></li>
    <li><a href="https://reactjs.org/">React.js</a></li>
    <li><a href="https://tailwindcss.com/">TailwindCSS</a></li>
  </ul>
</details>

<details>
  <summary>Server</summary>
  <ul>
    <li><a href="https://www.python.org/">Python</a></li>
    <li><a href="http://flask.palletsprojects.com/en/stable/">Flask</a></li>
    <li><a href="https://spacy.io/">SpaCy</a></li>
    <li><a href="https://pypi.org/project/beautifulsoup4/">BeautifulSoup</a></li>
    <li><a href="https://newsapi.org/">NewsAPI</a></li>

  </ul>
</details>

<details>
<summary>Database</summary>
  <ul>
    <li><a href="https://www.sqlite.org/">Sqlite</a></li>
    <li><a href="https://jena.apache.org/documentation/fuseki2/">Apache Jena Fuseki</a></li>
  </ul>
</details>

<details>
<summary>DevOps</summary>
  <ul>
    <li><a href="https://vercel.com/">Vercel</a></li>
    <li><a href="https://render.com/">Render</a></li>
  </ul>
</details>

<!-- Features -->

### :dart: Features

- **Authentication & Authorization (Clerk):** Handles user sign-in, sign-up, and session management with email/password, social logins, and passkeys. [Clerk Docs](https://clerk.dev/docs).
- **News Visualizer:** Enables users to scroll through articles, read them seamlessly, and open them in RDF format for structured data access.
- **SPARQL Querying:** Provides an interface for users to write and execute SPARQL queries, retrieving structured data with responses available in multiple formats, including JSON, JSON-LD, and RDFa.

<!-- Color Reference -->

### :art: Color Reference


| Color           | Hex                                                              |  
| --------------- | ---------------------------------------------------------------- |  
| Primary Color   |<span style="color:#3366FF;">#3366FF</span>|  
| Secondary Color |<span style="color:#DCEBFF;">#DCEBFF</span>|  
| Accent Color    |<span style="color:#0033CC;">#0033CC</span>|  
| Text Color      |<span style="color:#333333;">#333333</span>|  


<!-- Env Variables -->

### :key: Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`CLERK_SECRET_KEY`

`NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY`

<!-- Getting Started -->

## :toolbox: Getting Started

<!-- Prerequisites -->

### :bangbang: Prerequisites
Follow this tutorial in order to create a Clerk application for user management: [Clerk get started](https://clerk.com/docs/quickstarts/setup-clerk)

### :running: Run Locally

In order to run this project locally you will need to clone 3 repositories

#### nepr
This repository contains the frontend developed for this application
```bash
  git clone https://github.com/FanaruVictor/nepr.git
```

Go to the project directory

```bash
    cd nepr
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run dev
```

#### flask-ontology-app

This repository contains the backend developed for this application

```bash
  git clone https://github.com/SavRares/flask-ontology-app
```
Go to the project directory

```bash
    cd flask-ontology-app
```

Install dependencies

```bash
pip install -r requirements.txt
```

Start the server

```bash
export FLASK_APP=app.py
flask run
```

The project will be available on port 5000 by default

#### jena-fuseki-db-app

This repository contains a dockerfile which creates the fuseki database and it is needed for the deployment due to the free trial, as a workaround. To run locally:

```bash
  git clone https://github.com/SavRares/jena-fuseki-db-app
```

Go to the project directory

```bash
    cd flask-ontology-app
```

Run the dockerfile

```bash
docker build -t my-jena-fuseki-app .
docker run -d -p 3030:3030 my-jena-fuseki-app
```

To access the fuseki DB navigate to

```bash
http://localhost:3030
```

There you can upload the newsDCMI.rdf to the news datastore.

http://localhost:3030/#/dataset/news/upload => select files => select the newsDCMI.rdf file found in the git repo => upload all

<!-- Deployment -->

### :triangular_flag_on_post: Deployment
The deployment of this application is in three different steps depending on what part of the application you changed:

#### Frontend
If you added some modifications to the `nerp` repository, a pull request will be needes so the author of the repository can review the changes. Only after the author approves the changeset, it will be merged to the main branch and a deploy on vercel will be automatically triggered by the merge.

#### Backend

If you made changes to the `flask-ontology-app` repository, you will have to navigate to <a href="https://dashboard.render.com/">https://dashboard.render.com/</a> and re-deploy with the latest commit. 

An OpenAPI documentation can be found on this link: https://flask-ontology-app.onrender.com/apidocs/

### SPARQL DB

Changes are not expected to the `jena-fuseki-db-app` repository but if needed, after pushing to the git repo you will have to navigate to <a href="https://dashboard.render.com/">https://dashboard.render.com/</a> and re-deploy with the latest commit. 

Important! 
You will have to manually navigate to https://fuseki-sparql.onrender.com/#/dataset/news/upload
The data to be uploaded manually due to the free subscription to render deployment not allowing file storage. To do so, follow the instructions from the Run Locally section for jena-fuseki-db-app.

## :compass: Roadmap

- [x] Authentication and Authorization
- [x] News scrolling and visualization
- [x] SPARQL query page
- [ ] Add more data
- [ ] Extend ontology
<!-- Contributing -->

## :wave: Contributing

<a href="https://github.com/SavRares/Web-News-Provenance/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=SavRares/Web-News-Provenance" />
</a>

Contributions are always welcome!


## :warning: License
This project is distributed under the MIT License. 

<!-- Contact -->

## :handshake: Contact
Project Link: [https://github.com/SavRares/Web-News-Provenance](https://github.com/SavRares/Web-News-Provenance)
