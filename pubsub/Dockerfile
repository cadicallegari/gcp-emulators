FROM google/cloud-sdk:alpine

RUN apk --update add openjdk8-jre
RUN gcloud components install --quiet beta pubsub-emulator

ENTRYPOINT ["gcloud", "beta", "emulators", "pubsub"]
CMD ["start", "--host-port", "0.0.0.0:8085"]
