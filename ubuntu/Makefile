all: 14_04 15_10

14_04:
	$(MAKE) -C 14.04

15_10:
	$(MAKE) -C 15.10

clean:
	$(MAKE) -C 14.04 clean
	$(MAKE) -C 15.10 clean

push:
	$(MAKE) -C 14.04 push
	$(MAKE) -C 15.10 push

pull:
	$(MAKE) -C 14.04 pull
	$(MAKE) -C 15.10 pull
