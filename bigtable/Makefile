VERSION=latest
IMAGE=bigtable-emulator:$(VERSION)

build:
	docker build -t $(IMAGE) .

# default bigtable port is 8086
# do not forget to set these env vars
# export BIGTABLE_EMULATOR_HOST=[::1]:8086
run: build
	docker run --rm -p 2086:8086 $(IMAGE)
