FROM rust:1.61.0-bullseye

RUN apt-get update && \
    apt-get -y install git && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*
RUN rustup component add rls rust-analysis rust-src rustfmt clippy llvm-tools-preview
RUN cargo install cargo-edit cargo-llvm-cov cargo-watch