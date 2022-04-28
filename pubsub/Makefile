VERSION=latest
IMAGE=pubsub-emulator:$(VERSION)

build:
	docker build -t $(IMAGE) .

# default pubsub port is 8085
# do not forget to set these env vars
# export PUBSUB_EMULATOR_HOST=[::1]:8085
# export PUBSUB_PROJECT_ID=my-project-id
run: build
	docker run --rm -p 2085:8085 $(IMAGE)
