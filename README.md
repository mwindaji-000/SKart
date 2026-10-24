# SKart
SuperKart Prediction

## Run with Docker Compose

Start both the Flask prediction API and the Streamlit frontend:

```sh
docker compose up --build
```

Open the frontend at <http://localhost:8501>. Compose waits for the backend health check before starting the frontend. If port `8501` is already in use, set `FRONTEND_PORT` to an available host port.

To run the apps directly instead, start the backend on port `7860` and then run the frontend with `streamlit run frontend/app.py`. The frontend defaults to `http://localhost:7860`; set `BACKEND_URL` if the API is hosted elsewhere.
