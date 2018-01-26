FROM selenium/standalone-firefox:3.8.1-bohrium

ENV TINI_VERSION v0.16.1
ADD https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini /tini
RUN sudo chmod +x /tini

ENTRYPOINT ["/tini", "--", "/opt/bin/entry_point.sh"]
