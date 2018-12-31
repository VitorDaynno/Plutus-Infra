FROM ubuntu

RUN apt-get update && \
    apt-get install git -y && \
    apt-get install nodejs -y && \
    apt-get install npm -y

WORKDIR /app

RUN git clone https://github.com/VitorDaynno/Plutus-Service.git /app && \
    cd /app && \
    npm install --production && \
    chmod +x start.sh

CMD [ "/app/start.sh" ]