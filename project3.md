# MERN STACK IMPLEMENTATION

## The task for this project is to deploy a simple application that creates To-Do list

### STEP 1- Backend Configuration

1. I unpdated and upgraded the server package

  `sudo apt update`

  ![UpdateUbuntu](./Images3Project_MERN/Step1-UpdateUbuntu.PNG)

  `sudo apt upgrade`

  ![UpgradedUbuntu](./Images3Project_MERN/Step1-UpgradedUbuntu.PNG)


 2. To get the location of the Node.js software,

  `curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -`

  ![LocateNodeJs](./Images3Project_MERN/Step1-Install_NodeJS.PNG)


 3. Install Node.Js

  `sudo apt-get install -y nodejs`

  ![InstallNodeJs](./Images3Project_MERN/Step1-Install_NodeJS.PNG)


 4. Checked the version of Node and NPM

  `node -v`

  `npm -v`

  ![NodeNPMV](./Images3Project_MERN/Step1-Checked_NodeNpm_Version.PNG)


 5. Created a new directory 'Todo', changed directory to 'Todo' and initialised the task

   `mkdir Todo`

   `cd Todo`

   `npm init`

   ![InitialisedProjectMern](./Images3Project_MERN/Step1-Initialise_Project.PNG)


 6. Then checked for Package.Json

   ![CheckedPackageJson](./Images3Project_MERN/Step1-Check_for_PackageJson.PNG)  


 ### Install ExpressJs

 7. Installed ExpressJs

   `npm install express`

   ![InstallExpress](./Images3Project_MERN/Step1-Install_ExpressJs.PNG)


 8. Created file index.js

   `touch index.js`

   ![CreatedIndexJs](./Images3Project_MERN/Step1-Create_Index.Js_File.PNG)


 9. Installed dotenv

   `npm install dotenv`

   ![InstalledDotENV](./Images3Project_MERN/Step1-Install_dotenv.PNG)


 10. Checked server status

   `node index.js`

   ![ServerStatus](./Images3Project_MERN/Step1-Server_Running_On_Port5000.PNG)


 11. Access server on Public IP

   ![ExpressJs](./Images3Project_MERN/Welcome2Express.PNG)


 12. Created a new directory names ROUTES and changed directory to ROUTES

   `mkdir routes`
   `cd routes`

   ![Md_Cd_Routes](./Images3Project_MERN/CreateDir_Change2Routes.PNG)


 13. Create a file api.js and open to save lines of code

  `touch api.js`

  `vim api.js`


  ![OpenApiJs](./Images3Project_MERN/CreatedNewFile_api_OpenwithVim.PNG)

    
 14. Install mongoose

   `npm install mongoose`

   ![Mongoose](./Images3Project_MERN/Installed_Mongoose.PNG)

 15. Created a new file MODELS and chnaged directory to MODELS

   `mkdir models`

   `cd models`

   ![mk_cdModels](./Images3Project_MERN/CreatedModels_CDModels.PNG)

 16. Created todo.js file

   `touch todo.js`
   
   ![CreatedFileTodo](./Images3Project_MERN/CreatedFile_TodoJs.PNG)

 17. Opened  file todo.js

   `vim todo.js`

   ![OpenedTodo.js](./Images3Project_MERN/OpenedModelsFile_Todo.js_with_vim.PNG)

 18. Update and Open api.js in routes directory

  `vim api.js`

   ![OpenApi.Js](./Images3Project_MERN/Open_api.js_Routesdir.PNG)

 ### MongoDB Database

 19. Create a file '.env' in Todo and open the file.

  `touch .env`

  `vi .env`
  
  ![Createdotenv](./Images3Project_MERN/Step5-Created.envFile.PNG)


 20. Add the connection string to access the database

  ![Editdotenv_file](./Images3Project_MERN/Step5-AddString2.env.PNG)


 21. Update Index.js

   `vim index.js`

   Reveal content of index.js

   `cat index.js`

   ![UpdateIndexJs](./Images3Project_MERN/Step5-UpdateIndexJs_env.PNG)


 22. Start server using;

  `node index.js`

  ![StartServer](./Images3Project_MERN/Step5-StartServer_Status.PNG)


 ### Testing Backend Code without Frontend using RESTful API

 23.  Display a list of tasks – HTTP GET request

  ![ShowListofTasks](./Images3Project_MERN/Step6-API_Status.PNG)


  Add a new task to the list – HTTP POST request

  ![PostRequest](./Images3Project_MERN/Step6-PostRequest.PNG)
 

 ### Frontend Creation

 24. Create client directory in Todo directory

  `npx create-react-app client`

  ![CreateClientDir](./Images3Project_MERN/Step7-CreateDirClient.PNG)


 - Install Concurrently

  `npm install concurrently --save-dev`

  ![InstallConcurrently](./Images3Project_MERN/Step7-InstallAxios_on_client.PNG)


 - Install nodemon

  `npm install nodemon --save-dev`

  ![InstallNodemon](./Images3Project_MERN/Step7-InstallNodemon.PNG)

 
 25. Open and edit Package.Json

   `vi package.json`

   ![EditPackage.JsonFile](./Images3Project_MERN/Step7-EditedPackagejson.PNG)


 ### Configure Proxy in package.json

 26. Change directory to Client and Open Package.Json

  `cd client`

  `vi package.json`


 27. Add key value pair in package.json

  ![AddKVP](./Images3Project_MERN/Step7-AddKVP_in_packagejson.PNG)


 28. To ensure you are inside the Todo directory, run;

  `npm run dev`

  - Run `localhost:3000`   

  ![VerifyReactonLocalhost3000](./Images3Project_MERN/Step7-ShowReact.PNG) 

 
 ### Creating your React Components


 29. From the Todo directory, chance directory to client, and then to src

 `cd Todo && cd client && cd src`

 ![change_dir_to_src](./Images3Project_MERN/Step7-ChangeDir_client%26src.PNG) 


 30. Create and change directory to COMPONENTs

  `mkdir components`

  `cd components`

  ![Open_and_cdComponents](./Images3Project_MERN/Step7-Open%26cd_to_Components.PNG)


 31. Create 3 files 'Input, ListTodo, Todo' inside the directory COMPONENTs 

  `touch Input.js ListTodo.js Todo.js`

  - open input.js 

  ![CreateNewFile](./Images3Project_MERN/Step7-CreateNewFiles_InputListsTodo.PNG)


 32. Change directory back to client and install Axios

  `npm install axios`

  ![InstallAxios](./Images3Project_MERN/Step7-InstallAxios_on_client.PNG)


 33. Change to components and edit ListTodo.js

   `cd src/components`

   - `vi ListTodo.js`

   then edit Todo.js

   - `vi Todo.js`

   ![EditListTodo.Js](./Images3Project_MERN/Step8-EditedListTodo.PNG)

 34. Return to the src directory and edit the App.css file to delete the logo and adjust App.css

  `cd ..`

  `vi App.js`

  `vi App.css`

  - Also edit the index.css file

   `vim index.css`


 35. Return to Todo directory and run;

  `npm run dev`

  - Then reload the browser

   ![TheTodoWebPage](./Images3Project_MERN/FinalTodoWebPage.PNG)

