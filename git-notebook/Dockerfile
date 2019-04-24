FROM base-notebook:latest

USER root

RUN yum -y install nodejs && yum -y update nodejs
RUN jupyter labextension install @jupyterlab/git
RUN pip install jupyterlab-git
RUN jupyter serverextension enable --py jupyterlab_git

USER 1001
