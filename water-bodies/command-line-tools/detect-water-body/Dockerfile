FROM docker.io/python:3.10-slim

RUN apt-get update --yes && \
    apt-get install --yes libexpat1 && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

RUN pip install --no-cache-dir \
    rasterio \
    click \
    pystac \
    loguru \
    pyproj \
    shapely \
    scikit-image \
    pystac \
    rio_stac && \
    python -c "import rasterio"

ADD app.py /app/app.py

ENTRYPOINT []
