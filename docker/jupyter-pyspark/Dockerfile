FROM docker.io/jupyter/pyspark-notebook:x86_64-spark-3.5.0

# Install in the default python3 environment
RUN mamba install 'pytest' && \
    mamba install 'Pillow' && \
    pip install --no-cache 'pyAudioAnalysis' && \
    pip install --no-cache 'eyed3' && \
    pip install --no-cache 'pydub' && \
    pip install 'opencv-python' && \
    fix-permissions "${CONDA_DIR}" && \
    fix-permissions "/home/${NB_USER}"
