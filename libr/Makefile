all:

bea:
	$(MAKE) -C asm bea
	$(MAKE) -C anal bea

tab:
	$(MAKE) -C asm tab

olly:
	$(MAKE) -C asm olly

m68k:
	$(MAKE) -C asm m68k_net
	$(MAKE) -C anal m68k_net

zyan:
	$(MAKE) -C asm zyan

evm:
	$(MAKE) -C asm evm
	$(MAKE) -C anal evm
	$(MAKE) -C io evm
	$(MAKE) -C debug evm

clean:
	$(MAKE) -C asm clean
	$(MAKE) -C anal clean

bea-install:
	cp -f asm/p/asm_x86_bea.$(LIBEXT) $(R2PM_PLUGDIR)
	cp -f anal/p/anal_x86_bea.$(LIBEXT) $(R2PM_PLUGDIR)

tab-install:
	cp -f asm/p/asm_x86_tab.$(LIBEXT) $(R2PM_PLUGDIR)

olly-install:
	cp -f asm/p/asm_x86_olly.$(LIBEXT) $(R2PM_PLUGDIR)

m68k-install:
	cp -f asm/p/asm_m68k_net.$(LIBEXT) $(R2PM_PLUGDIR)
	cp -f anal/p/anal_m68k_net.$(LIBEXT) $(R2PM_PLUGDIR)

zyan-install:
	cp -f asm/p/asm_x86_zyan.$(LIBEXT) $(R2PM_PLUGDIR)

evm-install:
	cp -f asm/p/asm_evm.$(LIBEXT) $(R2PM_PLUGDIR)
	cp -f anal/p/anal_evm.$(LIBEXT) $(R2PM_PLUGDIR)
	cp -f io/p/io_evm.$(LIBEXT) $(R2PM_PLUGDIR)
	cp -f debug/p/debug_evm.$(LIBEXT) $(R2PM_PLUGDIR)

include ../options.mk
