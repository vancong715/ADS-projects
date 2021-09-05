# This Makefile generated from 'dtool'
CPP=				# or blan for nodebug
#CPP=yes		# or blank for C
#DEBUG=yes # or blank for nodebug

ifeq ($(strip $(COMDIR)),)
$(error error : app project name must be set)
else
VAR:=$(shell echo "COMDIR=$(COMDIR)")
endif

LSRC=$(wildcard ./*.l)
YSRC=$(wildcard ./*.y)

ifeq ($(strip $(CPP)),)
YOUT=../$(COMDIR)/src/conf_gram.c
LOUT=../$(COMDIR)/src/lexer.c
YOUTHXX=$(YOUT:%.c=%.h)
else
YOUT=../$(COMDIR)/src/conf_gram.cpp
LOUT=../$(COMDIR)/src/lexer.cpp
YOUTHXX=$(YOUT:%.cpp=%.hpp)
endif

#include ../../../mak/Lex.mak
include /d/dt/mak/lex.mk
