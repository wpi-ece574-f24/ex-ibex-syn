all: syn

syn:
	BASENAME=ibex_top \
	CLOCKPERIOD=10 \
	TIMINGPATH=/opt/cadence/libraries/gsclib045_all_v4.7/gsclib045/timing \
	TIMINGLIB=slow_vdd1v0_basicCells.lib \
	VERILOG='../rtl/ibex_alu.v ../rtl/ibex_csr.v ../rtl/ibex_if_stage.v ../rtl/ibex_register_file_ff.v ../rtl/ibex_branch_predict.v ../rtl/ibex_decoder.v ../rtl/ibex_load_store_unit.v ../rtl/ibex_compressed_decoder.v ../rtl/ibex_dummy_instr.v ../rtl/ibex_lockstep.v ../rtl/ibex_top.v ../rtl/ibex_controller.v ../rtl/ibex_ex_block.v ../rtl/ibex_multdiv_fast.v ../rtl/ibex_wb_stage.v ../rtl/ibex_core.v ../rtl/ibex_fetch_fifo.v ../rtl/ibex_multdiv_slow.v ../rtl/prim_generic_buf.v ../rtl/ibex_counter.v ../rtl/ibex_icache.v ../rtl/ibex_pmp.v ../rtl/prim_generic_flop.v ../rtl/ibex_cs_registers.v ../rtl/ibex_id_stage.v ../rtl/ibex_prefetch_buffer.v' \
	genus -f genus_script.tcl

clean:
	rm -rf outputs reports genus.log* genus.cmd* *~ fv

