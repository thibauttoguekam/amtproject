FROM jboss/wildfly:10.1.0.Final

MAINTAINER Frederic Fyfer <frederic.fyfer@heig-vd.ch>

RUN /opt/jboss/wildfly/bin/add-user.sh admin admin --silent

CMD ["/opt/jboss/wildfly/bin/standalone.sh", "-b", "0.0.0.0", "-bmanagement", "0.0.0.0"]

COPY ./apps-dist/ /opt/jboss/wildfly/standalone/deployments/