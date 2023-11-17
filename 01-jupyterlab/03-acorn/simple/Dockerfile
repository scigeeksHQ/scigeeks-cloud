FROM jupyter/tensorflow-notebook:python-3.10

RUN pip3 install boto3 
RUN mkdir $HOME/bin $HOME/data

RUN wget https://dl.min.io/client/mc/release/linux-amd64/mc \
  -O $HOME/bin/mc \
  && chmod +x $HOME/bin/mc
RUN echo "export PATH=\$PATH:\$HOME/bin/" >> ~/.bashrc