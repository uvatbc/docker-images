IMGTAG=uvatbc/nixnote2
IMGVER=v1

all: clean
	docker build -t $(IMGTAG):$(IMGVER) .

clean:
	-docker rmi $$(docker images | awk '{ if ($$1 == "$(IMGTAG)" && $$2 == "$(IMGVER)") { print $$1":"$$2 } }')

push:
	docker push $(IMGTAG):$(IMGVER)

pull:
	docker pull $(IMGTAG):$(IMGVER)

it:
	docker run --rm -it -v ~/src/github.com/:/mnt/src $(IMGTAG):$(IMGVER) /bin/bash
