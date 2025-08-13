### Upload to GitHub

### Azure Portal -> Add resource -> Web App + Database
1. Create a RG
- select location
- name it
- runtime stack - as per the requirements, this case Node 20
2. DB
- default Reccommended MONGODB
account name: exam-prep-server
database name: examp-prep-database
3. Cache for Redis -> No
4. Hosting Plan -> Basic

5. Create and wait for the deploy to finish

### 
1. When deployed GOTO RG -> WEBAPP -> Environment Varables to connect the DB
2. In the APP SETTINGS, copy the value of the default connection strign:

2. Check the url of the DB -> project/.env.sample -> Here is DATABASE_URL
3. Create an APP SETTING with that name and the value of the default connection string

4. Add another APP SETTING with DATABASE_NAME key and value -> the copied value of the database name when creating the app

5. APPLY THE CHANGES

### Deployment Center
1. Source -> GitHub
2. Select the REPO and the BRANCH
3. Add workflow
4. Auth type - User Assigned
5. SAVE

### Finalize
1. GitHub Action to be running
2. Create the screenshots required
3. .zip as per requirements and finish

