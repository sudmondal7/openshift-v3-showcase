FROM websphere-liberty:webProfile8

# Add binary deployment artifact to 'dropins' folder
#RUN wget --directory-prefix=/opt/ibm/wlp/usr/servers/defaultServer/dropins/ $BINARY_DEPLOYMENT_ARTIFACT_URL
#COPY app/* /opt/ibm/wlp/usr/servers/defaultServer/dropins/

RUN chmod -R a+rwx /opt/ibm/wlp/

COPY app/* /opt/ibm/wlp/usr/servers/defaultServer/dropins/

#RUN chmod -R a+rwx /opt/ibm/wlp/output/defaultServer/workarea

#RUN chmod a+rwx /opt/ibm/wlp/output/defaultServer/workarea/.sLock

# IBM WebSphere Liberty license must be accepted
ENV LICENSE $LICENSE
