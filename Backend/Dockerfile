FROM rust
RUN sudo apt-get update
RUN sudo apt-get -y upgrade
RUN sudo apt-get -y install libpq-dev
WORKDIR .
COPY . .
RUN  cargo install diesel_cli --no-default-features --features postgres
EXPOSE 8000
CMD [  "diesel" , "setup " && "cargo" , "run" ]

