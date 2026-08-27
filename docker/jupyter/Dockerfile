FROM python:3.11-slim

WORKDIR /workspace

# Install uv
COPY --from=ghcr.io/astral-sh/uv:latest /uv /uvx /bin/

# Install JupyterLab, Python kernel, and widgets
RUN uv pip install --system \
    jupyterlab \
    ipykernel \
    ipywidgets

# Make project source importable
ENV PYTHONPATH=/workspace/src

EXPOSE 8888

CMD ["jupyter", "lab", \
     "--ip=0.0.0.0", \
     "--port=8888", \
     "--no-browser", \
     "--allow-root", \
     "--ServerApp.token="]
