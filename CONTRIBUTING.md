# Contributing

> - [Running Locally](#running-locally)
> - [Creating a Pull Request](#creating-a-pull-request)
> - [Project Structure](#project-structure)

## Running Locally

1. Fork the main repo.

2. Clone your forked repo to your machine.

    ```bash
    git clone https://github.com/<your-username>/algorithm-visualizer.git    
    ```

3. Install [Docker](https://docs.docker.com/install/), if not already installed.

4. Install dependencies, and run the server.

    ```bash
    cd algorithm-visualizer

    npm install
    
    npm run dev
    ```
    
5. Open [`http://localhost:8080/`](http://localhost:8080/) in a web browser.

## Creating a Pull Request
  
1. Create a branch addressing the issue/improvement you'd like to tackle.

    ```bash
    git checkout -b my-problem-fixer-branch
    ```

2. Write some awesome code.

3. Commit the changes, and push them to `my-problem-fixer-branch` branch on your forked repo.

    ```bash
    git add .
    
    git commit -m "Explain my awesome changes"

    git push origin my-problem-fixer-branch
    ```

4. Create a pull request from `my-problem-fixer-branch` branch on your forked repo to `master` branch on the main repo.

## Project Structure

- **app/** wraps the backend and frontend servers.
- **bin/** contains executables.
- **branding/** contains representative image files.
- **build/** is where compiled files are located.
    - **backend/** contains the compiled backend server.
    - **frontend/** contains the compiled frontend server.
- **src/** contains source codes.
    - **backend/** contains the source code of the backend server.
        - **apis/** defines outgoing API requests.
        - **common/** contains commonly used files.
        - **controllers/** routes and processes incoming requests.
        - **public/** is where the backend server outputs.
            - **algorithms/** is cloned [`algorithm-visualizer/algorithms`](https://github.com/algorithm-visualizer/algorithms) repo.
            - **codes/** is where users' codes are uploaded to
            - **tracers/** is cloned [`algorithm-visualizer/tracers`](https://github.com/algorithm-visualizer/tracers) repo.
    - **frontend/** contains the source code of the frontend server.
        - **apis/** defines outgoing API requests.
        - **common/** contains commonly used files.
        - **components/** defines React components.
        - **core/** is in charge of visualization.
            - **datas/** manages visualization data.
            - **renderers/** renders visualization data.
        - **reducers/** contains Redux reducers.
        - **skeletons/** contains skeleton files to be shown in the code editor.
        - **static/** contains static files to be served.
