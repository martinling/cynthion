top.bit: top.py analyzer.py
	python top.py -o top.bit

load: top.bit
	apollo configure top.bit

flash: top.bit
	apollo force-offline
	apollo flash-erase
	apollo flash-program top.bit

clean:
	rm top.bit
