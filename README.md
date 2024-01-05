# codecademy-ecommerce-pern-app
PERN app to provide typical functionality found in an ecommerce website.  Users can create accounts, view products, add products to a cart, and place/view orders.

## Running the app
To run locally, `npm install`, then `npm run dev`

This project requires a [PostgreSQL](https://www.postgresql.org/) database to be running locally.  Reference the ERD diagram located in the `resources` folder of this repo to view the structure of the tables.  You can use [pgAdmin](https://www.pgadmin.org/) to interact with the database manually. 

This repo includes an `example.env` file that contains important environment variables for reference.  Make sure to create a `.env` file and include all variables found in the `example.env` file, replacing the example values with those specific to your environment/needs.

To easily populate your database with the requisite tables, `npm run create-db`.  This will create tables in your database if they do not already exist.  The configuration for this script can be found in the  `setupDatabase.js` file located in the server folder of this project.

Once the app is running locally, you can access it in a browser at `http://localhost:<your-port>`

## Running the app with Render
Create a new Render web service.

For the "Build Command", use `npm install --legacy-peer-deps`

For the "Start Command", use `npm run create-db && npm run dev`

Modify the `example.env` file within this repository to match your Render or manually set-up PostgreSQL instance host. You may also set Render environment variables for PGHOST and PGPORT when configuring the web service.

## Resources
- [REST Architecture](https://www.codecademy.com/articles/what-is-rest)
- [Using pgAdmin](https://www.pgadmin.org/docs/pgadmin4/development/getting_started.html)
- [React Documentation](https://reactjs.org/docs/getting-started.html)
- [Redux Documentation](https://redux.js.org/)
- [Redux Toolkit Documentation](https://redux-toolkit.js.org/)

## Options for Extension
- Add the ability to save payment methods for future purchases
- Add ability to favorite products for later
- Add ability to share product/purchase on social media
- Create a CMS for managing products and other administrative data
