# 📝 DEPLOYMENT TASKS
### ✔ Easy

## Define “environment variable”

Environment variable uses for store the secrets. never hardcode the secrets.

## Define “production environment”

Production is a live server. we develop the app or code in local, then move to stage for testing/QA, once we ensure our app or code is ready to live, we deploy it to the prod server. production environment expose our app or code to internet or live.

### ✔ Medium

## Write what will go inside your .env file for FastAPI

Example:

DB_HOST=
DB_PORT=
DB_USER=
DB_PASSWORD=
SECRET_KEY=
API_KEY=
KEY-NAME=
AWS_KEY=
8x8_key=
OPENAI_KEY=
SENDGRID_KEY=
TINY_URL_KEY=

### ✔ Hard

## Describe your 3-environment setup for future deployment:

Local laptop (dev) - First, we build our app in local, create a project workplace and folder structure, then write a code like business logic, APIs, DB queries, models, schemas, services, utils, etc., then we run the app in our local and test it, if its working we move it to the dev server.
Cloud VM staging  - after we complete the dev, next step is move to stage, because before we going to deploy it on production, we should test it properly with testcases, real inputs, multiple scenarios, find errors, find bugs, find defects, etc., these things handle by our QA, they report the bugs and issues to us, we need to fix it, after that everythings are working without any bugs or errors, we heading to next.

Cloud VM production  - once both dev and stage are working, then deploy those changes in prod server, those two are only for our implementations and confirmations, dev for build and stage for test, now this one is real phase of the project, how users access or use our
app? they should use our dev? or stage? No! they use our production server, it has the real database, APIs, and server.
So, production is live server, users can access it everywhere.
