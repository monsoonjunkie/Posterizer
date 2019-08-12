# Posterizer

Posterizer is a full stack LAMP & React shopping cart app demo.

## Techonologies Used

### Front-end
React.js, JavaScript, HTML5, CSS3, React, Bootstrap

### Back-end

PHP, MySQL, phpMyAdmin

## About the store

The store sells various posters from video games, movies, and comics. Users can pick and add, remove, and checkout items from their cart.

## Getting Started

1. Fork this repository to your GitHub account and clone the fork to your local directory.
2. Check out a `dev` branch and push it to `origin`.
    ```
    git push origin dev
    ```
3. Install all dependencies in `package.json` with NPM.
    ```
    npm install
    ```
4. Add the `posterizer.localhost` site to Apache by copying the provided virtual host configuration in the `server` directory to `/etc/apache2/sites-available`.
    ```
    sudo cp server/posterizer.localhost.conf /etc/apache2/sites-available
    ```
5. Enable the `posterizer.locahost` site.
   ```
   sudo a2ensite posterizer.localhost
   ```
6. Restart the Apache web server.
   ```
   sudo service apache2 restart
   ```
7. Test that the virtual host is working by sending an HTTP request to `http://posterizer.localhost`. You should receive `200 OK` response containing an HTML document with the title of "Posterizer".
   ```
   http get http://posterizer.localhost
   ```

## Features

There are [Markdown](https://guides.github.com/features/mastering-markdown/) files located in the `features` directory of this project that contain useful links and task lists for each feature of the application.

For each Markdown file, create a new Issue on your fork's GitHub repository and paste the content of the Markdown file into the **first** comment box. Give the Issue a clear title (usually the heading at the top of the Markdown file).

**Note**: GitHub automatically assigns Issue numbers when you open them. The numbers that GitHub gives your Issues are not meaningful in any way other than unique identification, so the order that you open Issues doesn't really matter. It _does_ matter what order you work on each feature for the project. The name of each Markdown file in `features` includes a number designating the order in which they should be implemented.

As you work through each task of a given feature, make a commit. It's good to get into the habit of making incremental progress on a project. Each commit message that you write should be concise, but descriptive enough that another developer can guess what you did in the code without having to actually read the code.

## NPM Scripts

- `dev` - Start Webpack Dev Server at port `localhost:3000`
- `build` - Run Webpack to build the React client into `server/public`.
