FROM debian

COPY . ~

RUN apt update && apt install -y openssh-server procps && apt-get install python3 && apt-get install python3-pip && python3 -m pip install --user ansible && export PATH="/root/.local/bin:$PATH"

CMD ["python3", "hello-world.py"]