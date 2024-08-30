# ABOUT PROJECT

This is the starter pack for `Rails`/`React` with `Vite` project. This is just a starter pack and you need to add additional `gems` and `packages` as per your need and make changes to the existing configs.

## Prerequisites:
Make sure you have the following installed before running the application:
- `Ruby`: `3.2.1`
- `NodeJs`: `20.3.1`
- `Rails`: `7.0.8`
- `MySql`
- `Yarn`/`npm`
- `Git`

## How to use?

1. Clone the repo
    ```bash
    git clone https://github.com/ajayamishra/rails_react_starter_pack.git
    ```
2. Install dependencies
    ```bash
    bundle install #To install gems for rails application
    yarn install #To install packages for React application
    ```
3. Change `DB` config (`config/database.yml`)
    ````bash
    #Change for all development, test and production environments
    username: <%= ENV['DB_USERNAME']||'root' %>
    password: <%= ENV['DB_PASSWORD']||'' %>
    host: <%= ENV['DB_HOSTNAME']||'127.0.0.1' %>
    port: <%= ENV['DB_PORT']||'3306' %>
    database: react_rails_starter_development
    ````
4. Create `Database`
    ```bash
    bin/rails db:create #This creates DB in MySQL, make sure your DB Server is running
    ```
5. Start Application
    ```bash
    To run Client: bin/vite dev
    To run Server: bin/rails s
    To run both: bin/dev
    ```
6. Use Application
    ```bash
    Access app from http://127.0.0.1:5100
    ```