FROM google/cloud-sdk:alpine

RUN gcloud components update beta

ENTRYPOINT ["gcloud", "beta", "emulators", "bigtable", "--quiet"]
CMD ["start", "--host-port", "0.0.0.0:8086"]
