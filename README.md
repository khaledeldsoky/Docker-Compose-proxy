## Creating a single HAProxy and two Apache containers with Docker compose

    In this porject we will create two identical Apache servers and one HAProxy container.

    When we want to access our website, we will be calling HAProxy, not the Apache servers. HAProxy will divert traffic to Apache servers in "round-robin" fashion.

    HTTP Request goes to HAProxy container.

    HAProxy container goes either Apache container 1 or 2.

    Response is served by Apache container 1 or 2.

    To run the project , make sure your are in the directory compose file and run this command
    ```bash
    docker compose up
    ```
    
    Go to your browse and put your ip and proxy port like this 
    ```bash
    [your-ip]:8080
    ```

    Refresh your browse some times you well see different web sites
