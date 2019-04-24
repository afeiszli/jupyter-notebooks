FROM base-notebook:latest

USER root

RUN apt-get -y install nodejs && apt-get -y update nodejs
RUN jupyter labextension install @jupyterlab/git
RUN pip install jupyterlab-git
RUN jupyter serverextension enable --py jupyterlab_git

USER 1001
