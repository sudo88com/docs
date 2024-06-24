# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

The site is automatically deployed using GitHub Actions. The output is available at [https://sudo88com.github.io/docs/Intro/](https://sudo88com.github.io/docs/Intro/).

### Local Development

The website is set up to use GitHub Actions for continuous integration and deployment. To run the website locally for development, follow these steps:

1. **Clone the Repository**:
```bash
$ git clone https://github.com/sudo88com/docs.git
$ cd docs
```

2. **Install Dependencies**:
```bash
$ npm install
```

3. **Start the Development Server**:
```bash
$ npm start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

To generate the static content for the website:

```bash
$ npm run build
```

This command creates static content in the `build` directory, which can be served using any static content hosting service.

# License
This project is licensed under the [MIT License](/LICENSE). See the LICENSE file for details.
