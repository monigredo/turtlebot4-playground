FROM gazebo

RUN apt-get update \
   && apt-get install -y python3-pip git \
   && pip install -U vcstools colcon-common-extensions \
 && rm -rf /var/lib/apt/lists/*

WORKDIR /workspace
COPY . /workspace

CMD ["bash"]
