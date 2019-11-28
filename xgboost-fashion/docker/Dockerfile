FROM jupyter/datascience-notebook
USER root
COPY docker/requirements.txt /tmp/
RUN pip install -r /tmp/requirements.txt
RUN jupyter contrib nbextension install
RUN R -e "install.packages('FactoMineR', repos='http://cran.irsn.fr/')"
RUN R -e "install.packages('factoextra', repos='http://cran.irsn.fr/')"
RUN R -e "install.packages('ggplot2', repos='http://cran.irsn.fr/')"
RUN R -e "install.packages('corrplot', repos='http://cran.irsn.fr/')"
RUN R -e "install.packages('psych', repos='http://cran.irsn.fr/')"
RUN R -e "install.packages('dplyr', repos='http://cran.irsn.fr/')"
RUN R -e "install.packages('hrbrthemes', repos='http://cran.irsn.fr/')"
