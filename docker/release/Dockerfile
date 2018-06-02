FROM yinghuiwang/todobackend-base:latest
MAINTAINER Eric Wang <eric.z.wang@ericsson.com>


# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse
