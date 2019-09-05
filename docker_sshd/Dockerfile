FROM alpine:latest

RUN apk update && \
    apk add bash git openssh rsync augeas shadow

RUN echo "root:cynergyruas" | chpasswd

RUN ssh-keygen -f /etc/ssh/ssh_host_rsa_key -N '' -t rsa

RUN echo "ssh" >> /etc/securetty && echo "ALL : ALL" >> /etc/hosts.allow

COPY sshd_config /etc/ssh/sshd_config

EXPOSE 22

CMD [ "/usr/sbin/sshd" , "-D"]
