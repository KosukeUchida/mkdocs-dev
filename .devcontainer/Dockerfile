FROM mcr.microsoft.com/vscode/devcontainers/python:3.12-bookworm

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    git \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# pipをアップグレード
RUN pip install --upgrade pip

# 作業ディレクトリを設定
WORKDIR /workspace

# requirements.txt からパッケージをインストール
COPY requirements.txt .
RUN pip install -r requirements.txt

# Default command
CMD ["/bin/bash"]