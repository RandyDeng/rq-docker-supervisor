FROM python:3

ENTRYPOINT ["/bin/bash"]

# Install Python dependencies
RUN pip install rq
RUN pip install supervisor

# Spawn workers according to config
CMD ["-c", "supervisord -c /usr/src/workers/supervisord.conf -n"]
