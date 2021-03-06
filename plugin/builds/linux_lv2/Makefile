ifndef CONFIG
  CONFIG=Release
endif

all: binary ttl_generator lv2

binary:
	$(MAKE) -f Makefile.binary CONFIG=$(CONFIG) DEBCXXFLAGS="$(DEBCXXFLAGS)" DEBLDFLAGS="$(DEBLDFLAGS)"

ttl_generator:
	$(MAKE) -f Makefile.ttl_generator CONFIG=$(CONFIG)

lv2: ttl_generator binary
	./lv2_ttl_generator build/Vitality+Minus.so
	mkdir -p Vitality+Minus.lv2
	cp build/Vitality+Minus.so Vitality+Minus.lv2
	mv *.ttl Vitality+Minus.lv2

clean:
	$(MAKE) clean CONFIG=$(CONFIG) -f Makefile.binary
	$(MAKE) clean CONFIG=$(CONFIG) -f Makefile.ttl_generator
	rm -rf build
	rm -rf Vitality+Minus.lv2
