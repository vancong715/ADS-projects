# Do not delete project info below
#!! s0 	=	 ads0 ;
###############################
COMDIR=app

ifeq ($(TARGET),clean)
modules := ./$(COMDIR) ./lex
MSGB=clean
else
modules := ./lex ./$(COMDIR)
MSGB=build
endif

.PHONY: all $(modules) clean start

all: start $(modules)
	@echo --\> Build $(APPNAME) done
	@echo \ 

clean: start $(modules)
	@echo --\> Clean $(APPNAME) done
	@echo \ 

$(modules):
	@echo ---\>$@
	$(MAKE) --directory=$@ $(TARGET) COMDIR=$(COMDIR) PROJ=$(APPNAME)

start:
	@echo --\> Start $(MSGB) $(APPNAME)
