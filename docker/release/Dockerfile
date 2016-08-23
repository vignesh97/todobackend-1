FROM tzahif1/todobackend-base:latest
MAINTAINER Tzahi <tzahif1@gmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse