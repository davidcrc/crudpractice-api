mkdir crudPractice-api
cd crudPractice-api
git init
mkdir controllers
code .


npm init -y
npm install express body-parser pg knex dotenv helmet cors morgan
npm install nodemon --save-dev


brew services start postgresql
createdb crud-practice-1


CREATE TABLE testtable1 (
 id serial PRIMARY KEY,
 first VARCHAR(100),
 last VARCHAR(100),
 email text UNIQUE NOT NULL,
 phone VARCHAR(100),
 location VARCHAR(100),
 hobby VARCHAR(100),
 added TIMESTAMP NOT NULL
);