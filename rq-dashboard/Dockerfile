FROM python:3

ENTRYPOINT ["/bin/bash"]

# Install Python dependencies
RUN pip install rq-dashboard

CMD ["-c", "rq-dashboard -H redis"]