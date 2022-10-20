FROM debian

RUN apt update && apt install -y openssh-server procps && \
touch test_file.txt; apt install -y python3 && apt install -y python3-pip && \
python3 -m pip install --user ansible

RUN sed -i '1iPATH="${PATH}:/root/.local/bin"' ~/.profile