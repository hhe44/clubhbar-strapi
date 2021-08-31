# Club Hbar Strapi
This will be the strapi that provides content data via API requests to the Club Hbar site.

# Local Setup (Windows)
1. Install Postgresql [here](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads), select the latest Windows x86-64 installer
2. Run the installer, your data directory should be `C:\Program Files\PostgreSQL\<VERSION>\data`.
3. The installer will prompt you for a password, **this will be used to access superuser postgres**. Set it to *password* for minimal work. 
4. Have the port listen at 5432, which the installer defaults to.
5. When asked to select the locale for the new database cluster, just select **Default Locale**.
6. Run through the installation. Upon completion, open the pgAdmin application. Whenever pgAdmin requests for a password, enter `password` or whatever was inputted in step 3. 
7. Click on **Servers** on the top-left, then right click on **PostgreSQL** and select **Connect Server**. You may be prompted to do so without right clicking. Enter the password in Step 6 to continue. 
8. With your postgresql server up, download the repository, cd into it and run npm start. You may want to use the commands below to expedite the process: <br>
`git clone https://github.com/hhe44/clubhbar-strapi.git` <br>
`cd clubhbar-strapi` <br>
`npm install` <br>
`npm run develop`
9. Once strapi is up, manage the project at http://localhost:1337/admin

# Heroku Deployment
[See this guide](https://strapi.io/documentation/developer-docs/latest/setup-deployment-guides/deployment/hosting-guides/heroku.html)