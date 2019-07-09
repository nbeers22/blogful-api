# Express API Boilerplate!

This is a boilerplate project used for starting new projects!

## Set up

Complete the following steps to start a new project (NEW-PROJECT-NAME):

1. Clone this repository to your local machine SSH: `git clone git@github.com:nbeers22/express-api-boilerplate.git` or HTTPS: `https://github.com/nbeers22/express-api-boilerplate.git`
2. `cd` into the cloned repository
3. Make a fresh start of the git history for this project with `rm -rf .git && git init`
4. Install the node dependencies `npm i`
5. Move the example Environment file to `.env` that will be ignored by git and read by the express server `mv example.env .env`
6. Edit the contents of the `package.json` to use YOUR-PROJECT-NAME instead of `"name": "express-boilerplate",`

## Scripts

Start the application `npm start`

Start nodemon for the application `npm run dev`

Run the tests `npm test`

Run all migrations `npm run migration`

Run specific migration `npm run migration -- 1`

Seed Database `psql -U user_name -d database_name -f ./path-to-seed-file.sql`

## Deploying

When your new project is ready for deployment, add a new Heroku application with `heroku create`. This will make a new git remote called "heroku" and you can then `npm run predeploy` which will run an npm audit and then `npm run deploy` which will push to this remote's master branch.