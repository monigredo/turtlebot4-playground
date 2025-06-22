FROM gazebo

RUN apt-get update \
   && apt-get install -y python3-pip \
   && pip install -U vcstool colcon-common-extensions \
 && rm -rf /var/lib/apt/lists/*

WORKDIR /workspace
COPY . /workspace

CMD ["bash"]
