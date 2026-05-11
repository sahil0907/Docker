FROM python:3.11-slim
RUN useradd -m sahil
WORKDIR /home/sahil/app
COPY --chown=sahil:sahil requirements.txt ./
RUN pip install --no-cache-dir -r requirement.txt
COPY --chown=sahil:sahil . ./
USER sahil
ENTRYPOINT [ "python3", "app.py" ]
