# Makefile

ROOTDIR = ../../..
include $(ROOTDIR)/config.mk

SUBDIRS = $(filter-out Interface/, $(sort $(dir $(wildcard */))))
CLEANSUBDIRS = $(addsuffix .clean, $(SUBDIRS))

.PHONY: ChangeObserverExample  SimpleApp  SimpleUse  Win32DllTempl
all: ChangeObserverExample  SimpleApp  SimpleUse  Win32DllTempl

ChangeObserverExample:
	@echo
	@echo Making all in subdirectory $@...
	$(MAKE) -C ChangeObserverExample

HelloView:
	@echo
	@echo Making all in subdirectory $@...
	$(MAKE) -C HelloView

HelloViewApp:
	@echo
	@echo Making all in subdirectory $@...
	$(MAKE) -C HelloViewApp

MFCExtTempl:
	@echo
	@echo Making all in subdirectory $@...
	$(MAKE) -C MFCExtTempl

SimpleApp:
	@echo
	@echo Making all in subdirectory $@...
	$(MAKE) -C SimpleApp

SimpleUse:
	@echo
	@echo Making all in subdirectory $@...
	$(MAKE) -C SimpleUse

Win32DllTempl:
	@echo
	@echo Making all in subdirectory $@...
	$(MAKE) -C Win32DllTempl

clean:	$(CLEANSUBDIRS)

$(CLEANSUBDIRS):
	@cd $(basename $@) ; $(MAKE) clean


