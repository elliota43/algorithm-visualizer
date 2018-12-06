# Project Details

> #### Table of Contents
> - [Project Structure](#project-structure)
> - [Directory Structure](#directory-structure)
>   - [algorithms](#algorithms)
>   - [tracers](#tracers)
>   - [algorithm-visualizer](#algorithm-visualizer)

## Project Structure

The project [algorithm-visualizer](https://github.com/algorithm-visualizer) consists of the following 3 repos.

- [algorithms](#algorithms) contains public algorithms shown on the sidebar.

- [tracers](#tracers) generates visualization libraries for each supported language based on the specifications, and executes users' codes to extract visualization data.

- [algorithm-visualizer](#algorithm-visualizer) contains the frontend server written in React and the backend server written in Node.

## Directory Structure

### [algorithms](https://github.com/algorithm-visualizer/algorithms)

### [tracers](https://github.com/algorithm-visualizer/tracers)

### [algorithm-visualizer](https://github.com/algorithm-visualizer/algorithm-visualizer)

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
