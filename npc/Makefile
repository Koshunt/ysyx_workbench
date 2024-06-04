all:
	@echo "Write this Makefile by your self."
	verilator --c --exe --build --Wall --trace test.cpp test.v
sim:
	$(call git_commit, "sim RTL") # DO NOT REMOVE THIS LINE!!!
	@echo "Write this Makefile by your self."

include ../Makefile
