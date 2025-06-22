# Use the Gazebo Harmonic base image. The "-jazzy" tag referenced in the
# initial workflow no longer exists, so pin to the generic Harmonic image
# at the desired timestamp.
FROM ghcr.io/gazebo-release/gz-harmonic:2025-05

RUN apt-get update \
 && apt-get install -y --no-install-recommends \
    python3-vcstool \
    python3-colcon-common-extensions \
 && rm -rf /var/lib/apt/lists/*

WORKDIR /workspace
COPY . /workspace

CMD ["bash"]
