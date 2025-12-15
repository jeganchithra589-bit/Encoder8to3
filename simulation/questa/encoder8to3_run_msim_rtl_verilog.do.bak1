transcript on
if {[file exists rtl_work]} {
	vdel -lib rtl_work -all
}
vlib rtl_work
vmap work rtl_work

vlog  -work work +incdir+D:/Digi\ lab/encoder8to3 {D:/Digi lab/encoder8to3/encoder8to3.v}

vlog  -work work +incdir+D:/Digi\ lab/encoder8to3 {D:/Digi lab/encoder8to3/encoder8to3.v}

vsim -t 1ps -L altera_ver -L lpm_ver -L sgate_ver -L altera_mf_ver -L altera_lnsim_ver -L cyclonev_ver -L cyclonev_hssi_ver -L cyclonev_pcie_hip_ver -L rtl_work -L work -voptargs="+acc"  encoder8to3

add wave *
view structure
view signals
run -all
