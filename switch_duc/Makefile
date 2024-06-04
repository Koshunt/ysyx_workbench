all:
	build run wave
	#@echo "Write this Makefile by your self."
build:
	verilator --cc --exe --build --Wall --trace  $(filter %.cpp,$(MAKECMDGOALS)) $(filter %.v,$(MAKECMDGOALS))
clean:
	rm -rf obj_dir
wave:
	gtkwave simx.vcd

sim:
	$(call git_commit, "sim RTL") # DO NOT REMOVE THIS LINE!!!
	@echo "Write this Makefile by your self."
	verilator --cc --exe --build --Wall --trace  test.cpp top.v
run:
	obj_dir/V$(basename $(filter %.v,$(MAKECMDGOALS)))

include ../Makefile
