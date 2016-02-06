all: 4 5 5_32

4:
	make -C qt4

5:
	make -C qt5

5_32:
	make -C qt5_32

clean:
	make -C qt4 clean
	make -C qt5 clean
	make -C qt5_32 clean

push:
	make -C qt4 push
	make -C qt5 push
	make -C qt5_32 push

pull:
	make -C qt4 pull
	make -C qt5 pull
	make -C qt5_32 pull
