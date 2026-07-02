# Start from an image that already has the GNU C++ toolchain installed
FROM gcc:14

# All following commands run inside /app in the container
WORKDIR /app

# Copy main.cpp from your machine into the container's /app directory
COPY main.cpp .

# Compile it while the image is being built
RUN g++ -Wall -Wextra -o hello main.cpp

# When a container starts from this image, run the compiled program
CMD ["./hello"]
