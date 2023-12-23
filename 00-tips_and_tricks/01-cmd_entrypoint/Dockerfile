FROM ubuntu

RUN apt-get update && apt-get install -y figlet

COPY ./start.sh .
RUN chmod +x start.sh

ENV TEXT="Hello SciGeeks"

ENTRYPOINT [ "/start.sh" ]

CMD figlet -f digital $(cat /tmp/text.txt)