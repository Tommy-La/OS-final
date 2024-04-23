# Challenge 3

## Steps:
1. **Download and Extract Files:**
   - Download the challenge3 folder from D2L and extract it to your desired location.

2. **Setup Docker Compose and Environment Variables:**
   - Set up the `docker-compose.yml` and `variables.env` files according to your project requirements.

3. **Modify Dockerfile:**
   - Navigate to the `docker/api/Dockerfile`.
   - Change the line:
     ```
     COPY docker/api/package*.json ./ 
     ```
     to:
     ```
     COPY ./package*.json ./
     ```

4. **Build and Run Docker Compose:**
   - Open a terminal.
   - Run the command:
     ```
     docker-compose up --build
     ```

# Challenge 4

## Steps:
1. **Modify Docker Compose File:**
   - Open the `docker-compose.yml` file in a text editor.
   - Add the `scale` option to the `node-service` service definition and set it to `3`.

2. **Remove Port in Node Service:**
   - Remove the port mapping for the `node-service` in the `docker-compose.yml` file.

3. **Scale Node Service:**
   - Open a terminal.
   - Run the command:
     ```
     docker-compose up --scale node-service=3 -d
     ```
   This starts three instances of the node-service.

## Citations:
[1] "100+ Docker Concepts you Need to Know," [www.youtube.com](https://www.youtube.com/watch?v=rIrNIzy6U_g) (accessed Apr. 23, 2024).
[2] "Docker Tutorial for Beginners," [www.youtube.com](https://www.youtube.com/watch?v=pTFZFxd4hOI)
