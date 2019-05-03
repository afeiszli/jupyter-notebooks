FROM base-notebook:latest

COPY jupyter_notebook_config.py /opt/app-root/etc/jupyter_notebook_config.py
RUN pip install voila --pre
#RUN jupyter serverextension install --py voila
RUN jupyter serverextension enable --py voila
