FROM rust
sudo apt install libpq-dev
WORKDIR .
COPY . .
RUN  cargo install diesel_cli --no-default-features --features postgres
EXPOSE 8000
CMD [ "cargo","run","--release" ]

