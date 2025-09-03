# docker-and-containers
#Steps Followed
Installed and started Docker Desktop; verified the engine was running.

Created the project files: app.py, requirements.txt, Dockerfile, compose.yaml, .dockerignore, and README.md.

Declared dependencies (flask, redis) in requirements.txt.

Implemented a Flask app that connects to Redis, increments a hits counter, and returns “Hello World! I have been seen N times.”

Wrote a Dockerfile to containerize the Flask app (exposes port 5000 inside the container).

Created compose.yaml with three services:

web: Flask app, mapped host 8000 → 5000, depends on Redis.

redis: official Redis image with a named volume to persist the counter.

db: Postgres database mapped 5432 → 5432.

Built and started the stack; confirmed all containers were running in Docker Desktop.

Opened http://localhost:8000 and verified the counter increments on refresh.

Reviewed container logs in Docker Desktop and captured a logs screenshot.

(Optional) Confirmed Postgres connectivity using a database client.

Captured required screenshots: Containers view, browser page at http://localhost:8000, and logs view.

Created a GitHub repository, added all project files, and pushed the code.

Logged any issues encountered (e.g., missing dependencies, port conflicts, counter reset without volume) in the repo’s Issues tab with brief resolutions.

Prepared a one-page submission document embedding the three screenshots and the GitHub URL.

Stopped the stack and cleaned up after verification and documentation were complete.

