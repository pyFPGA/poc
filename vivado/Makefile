#!/usr/bin/make

COMMAND=vivado -mode batch -notrace -quiet -source

flow params:
	$(COMMAND) $@.tcl

version:
	echo "puts \$$tcl_version" | vivado -mode tcl -notrace -quiet

clean:
	rm -fr *.bit *.cache *.hw *.runs *.xpr *.jou *.ip_user_files
	rm -fr *.html *.log *.txt *.xml .Xil
