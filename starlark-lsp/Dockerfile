FROM golang:1.19.1-bullseye

ENV PORT="3000"

WORKDIR /root
RUN wget https://github.com/tilt-dev/starlark-lsp/archive/main.tar.gz
RUN tar xzf main.tar.gz
WORKDIR /root/starlark-lsp-main
RUN make install
CMD starlark-lsp start --address=":${PORT}"
