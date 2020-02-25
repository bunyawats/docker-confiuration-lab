FROM rabbitmq:3.8.1-management

RUN apt-get update && \
apt-get install -y curl unzip

RUN curl https://dl.bintray.com/rabbitmq/community-plugins/3.8.x/rabbitmq_delayed_message_exchange/rabbitmq_delayed_message_exchange-20191008-3.8.x.zip > rabbitmq_delayed_message_exchange-20191008-3.8.x.zip && \
unzip rabbitmq_delayed_message_exchange-20191008-3.8.x.zip && \
rm -f rabbitmq_delayed_message_exchange-20191008-3.8.x.zip && \
mv rabbitmq_delayed_message_exchange-20191008-3.8.x.ez plugins/

RUN rabbitmq-plugins enable rabbitmq_delayed_message_exchange