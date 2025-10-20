# Pin a Debian base so we have apt (and avoid Alpine recovery)
FROM mcr.microsoft.com/devcontainers/base:bookworm

# Install Tectonic (and latexmk + some TeX Live bits if you want them)
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        tectonic \
        latexmk \
        texlive-latex-recommended \
        texlive-latex-extra \
        texlive-fonts-recommended && \
    rm -rf /var/lib/apt/lists/*
