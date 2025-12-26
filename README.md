# java_palyground_docker
Javaを試すためのDocker環境

## Java Playground with Docker

This is a simple playground environment for learning Java using Docker.

### Prerequisites

- Docker
- Docker Compose

### How to Use

1.  **Start the container:**
    ```bash
    docker-compose up -d
    ```

2.  **Enter the container:**
    ```bash
    docker-compose exec java-playground bash
    ```

3.  **Compile your Java code:**
    The `src` directory is mounted in the container. You can compile your Java files like this:
    ```bash
    javac src/HelloWorld.java
    ```

4.  **Run your Java program:**
    After compiling, you can run the program. Make sure to specify the classpath.
    ```bash
    java -cp src HelloWorld
    ```

5.  **Edit your code:**
    You can edit the `.java` files in the `src` directory on your host machine. The changes will be reflected inside the container immediately. Just re-compile and re-run.

6.  **Stop the container:**
    ```bash
    docker-compose down
    ```
