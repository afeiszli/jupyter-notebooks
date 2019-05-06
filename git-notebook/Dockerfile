FROM base-notebook:latest

USER root
COPY setup_node.sh .
RUN chmod 777 setup_node.sh && ./setup_node.sh
#RUN source <(curl -sL https://rpm.nodesource.com/setup_10.x)
#RUN apt-get -y install nodejs && apt-get -y update nodejs
#RUN yum -y install gcc-c++ make
#RUN curl -sL https://rpm.nodesource.com/setup_10.x | sudo -E bash -
RUN yum -y install nodejs
RUN pip install jupyterlab --upgrade
RUN jupyter labextension install @jupyterlab/git
RUN pip install jupyterlab-git
RUN jupyter serverextension enable --py jupyterlab_git --sys-prefix

USER 1001
