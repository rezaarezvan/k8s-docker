FROM ubuntu:latest

RUN apt-get update && apt-get install -y \
    gcc \
    make

WORKDIR /home/reza/Code/k8s-docker/LAMS/

# Copy the entire project directory
COPY . .

# Run Makefile
RUN make

# Run the executable
CMD ["/home/reza/Code/k8s-docker/LAMS/output"]
