FROM base-notebook:latest

USER root
RUN source <(curl -sL https://rpm.nodesource.com/setup_10.x)
#RUN apt-get -y install nodejs && apt-get -y update nodejs
RUN yum -y install gcc-c++ make
RUN curl -sL https://rpm.nodesource.com/setup_10.x | sudo -E bash -
RUN yum -y install nodejs
RUN jupyter labextension install @jupyterlab/git
RUN pip install jupyterlab-git
RUN jupyter serverextension enable --py jupyterlab_git

USER 1001
