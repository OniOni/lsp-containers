FROM python:3.10

ENV PORT="3000"

RUN python -m pip install "python-lsp-server[all]"
CMD pylsp --tcp --port "${PORT}" --host 0.0.0.0
