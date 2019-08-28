all: Emblem.dxf

%.eps: %.svg
	inkscape -z -f $< -E $@

%.dxf: %.eps
	pstoedit -dt -f "dxf_s:-splineasbezier -mm" $< $@
