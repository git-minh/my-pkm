# 📚 my-pkm

Welcome to **my-pkm** – my personal knowledge management system built with Docusaurus. This project helps me organize, manage, and access all my important information efficiently.

## 🚀 Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### 📦 Prerequisites

Make sure you have [Node.js](https://nodejs.org/) installed on your machine.

### 🛠 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/git-minh/my-pkm.git
   cd my-pkm
   ```

2. Install the dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npx docusaurus start
   ```

   Your site is now running at `http://localhost:3000`!

## 📁 Project Structure

- **/docs**: Documentation files
- **/blog**: Blog posts
- **/src**: Source files for customization
- **/static**: Static assets like images and files

## ✨ Features

- **Documentation**: Organize your knowledge with structured documents.
- **Blog**: Keep track of your thoughts and ideas.
- **Customization**: Easily customize the look and feel of your site.

## 🤝 Contributing

This is a personal project, but if you have suggestions or improvements, feel free to open an issue or submit a pull request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Contact

Feel free to reach out if you have any questions or suggestions!

---

Happy documenting! ✍️
```

You can replace `https://github.com/git-minh/my-pkm.git` with your actual GitHub repository URL. This README provides a clear and friendly overview of your project, including installation instructions, project structure, and features.


---

# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

### Installation

```
$ yarn
```

### Local Development

```
$ yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```
$ yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

Using SSH:

```
$ USE_SSH=true yarn deploy
```

Not using SSH:

```
$ GIT_USER=<Your GitHub username> yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
