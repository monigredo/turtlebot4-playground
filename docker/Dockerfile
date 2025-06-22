FROM ghcr.io/gazebo-release/gz-harmonic-jazzy:2025-05

RUN apt-get update \
 && apt-get install -y --no-install-recommends \
    python3-vcstool \
    python3-colcon-common-extensions \
 && rm -rf /var/lib/apt/lists/*

WORKDIR /workspace
COPY . /workspace

CMD ["bash"]
