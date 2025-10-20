# Debian base so we have apt
FROM mcr.microsoft.com/devcontainers/base:bookworm

# TeX Live + latexmk (works with LaTeX Workshop)
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        latexmk \
        texlive-latex-base \
        texlive-latex-recommended \
        texlive-latex-extra \
        texlive-fonts-recommended \
        ghostscript && \
    rm -rf /var/lib/apt/lists/*
