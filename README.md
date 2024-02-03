### Setup

1.  Clone the repository

    ```bash
    git clone https://github.com/ProfNuru/flowise-clone.git
    ```

2.  Go into repository folder

    ```bash
    cd Flowise
    ```

3.  Install all dependencies of all modules:

    ```bash
    yarn install
    ```

4.  Build all the code:

    ```bash
    yarn build
    ```

5.  Run locally in development:

    -   Create `.env` file in `packages/server`
    -   Copy the contents of `packages/server/.env.example` and paste it in the `.env`
    -   Change the paths in the following environment variables in `.env`:
        -   DATABASE_PATH=/full_path_to_this_project/db
        -   APIKEY_PATH=/full_path_to_this_project/apikeys
        -   SECRETKEY_PATH=/full_path_to_this_project/secret
        -   LOG_PATH=/full_path_to_this_project/logs
            I have used example path for my windows PC
    -   Create the `logs` folder in the root of the project
    -   Run

            ```bash
            yarn dev
            ```

        You can now access the app on [http://localhost:3000](http://localhost:3000)

## 🔒 Authentication

To enable app level authentication, add `FLOWISE_USERNAME` and `FLOWISE_PASSWORD` to the `.env` file in `packages/server`:

```
FLOWISE_USERNAME=user
FLOWISE_PASSWORD=1234
```

## 🌱 Env Variables

Flowise support different environment variables to configure your instance. You can specify the following variables in the `.env` file inside `packages/server` folder. Read [more](https://github.com/FlowiseAI/Flowise/blob/main/CONTRIBUTING.md#-env-variables)

## 📖 Documentation

[Flowise Docs](https://docs.flowiseai.com/)
