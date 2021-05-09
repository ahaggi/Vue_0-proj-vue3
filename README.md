
 Install via vue official CLI

    npm install -g @vue/cli
    nvm install --lts

Then in the Vue projects, run 

    ´vue upgrade --next´

Create new project

    Alt1- Using Vite 
        https://vitejs.dev/guide/

        Vite requires Node.js version >=12.0.0.

        For production: the default build targets browsers that support native ESM via script tags. Legacy browsers can be supported via the official @vitejs/plugin-legacy - see the Building for Production section for more details

        ***  MAYBE USE THIS FOR DEV PURPOSE ONLY! ***

        To create a new project:

            `npm init @vitejs/app <project-name>`
            ´cd <project-name>´ 
            ´npm install´ 
            ´npm run dev´   ==>  http://localhost:3000/





    Alt2- Using vue create
        1- ´vue create <project-name>´

        2- Modify package.json 
            {
                "scripts": {
                    "serve": "vue-cli-service serve",
                    "build": "vue-cli-service build"
                }
            }
        3- finally
        ´npm run serve´ ==>  http://localhost:8080/




Setup vetur
vetur is a Vue tooling for VS Code, powered by vls
https://vuejs.github.io/vetur/guide/setup.html  