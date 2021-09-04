FROM tsl0922/ttyd

RUN apt update && apt install -y openssh-client

ENTRYPOINT ["/usr/bin/tini", "--"]
CMD ["ttyd", "bash"]