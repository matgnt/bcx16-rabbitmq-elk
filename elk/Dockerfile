FROM sebp/elk

WORKDIR ${LOGSTASH_HOME}
RUN bin/plugin install logstash-input-rabbitmq

COPY 60-rabbitmq.conf /etc/logstash/conf.d/

