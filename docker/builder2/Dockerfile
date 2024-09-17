FROM pablintino/builder2:dev


ARG BUILDER_INSTALLATION=/tools
ARG BUILDER_CUSTOM_CERTS=/etc/ssl/custom
ENV BUILDER_INSTALLATION=$BUILDER_INSTALLATION
ENV BUILDER_CUSTOM_CERTS=$BUILDER_CUSTOM_CERTS

COPY pbtn-infra-toolchain-metadata.json /opt/builder2/pbtn-infra-toolchain-metadata.json

RUN builder2 install -f /opt/builder2/pbtn-infra-toolchain-metadata.json -d $BUILDER_INSTALLATION
