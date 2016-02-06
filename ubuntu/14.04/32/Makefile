IMGTAG=uvatbc/ubuntu
IMGVER=14.04_32

all: clean
	docker build -t $(IMGTAG):$(IMGVER) .

clean:
	-docker rmi $$(docker images | awk '{ if ($$1 == "$(IMGTAG)" && $$2 == "$(IMGVER)") { print $$1":"$$2 } }')
	-docker rmi $$(docker images | awk '{ if ($$1 == "32bit/ubuntu" && $$2 == "$(IMGVER)") { print "32bit/ubuntu:14.04" } }')

push:
	docker push $(IMGTAG):$(IMGVER)

pull:
	docker pull $(IMGTAG):$(IMGVER)

it:
	-docker run --rm -it -v ~/code/:/mnt/code $(IMGTAG):$(IMGVER) /bin/bash
