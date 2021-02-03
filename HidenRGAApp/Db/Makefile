TOP=../..
include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE

#----------------------------------------------------
#  Optimization of db files using dbst (DEFAULT: NO)
#DB_OPT = YES

#----------------------------------------------------
# Create and install (or just install)
# databases, templates, substitutions like this
DB += asynRecord.db
DB += hiden_rga_global.db
DB += hiden_rga_bar.db
DB += hiden_rga_prfl.db
DB += hiden_rga_mid.db
DB += hiden_rga_ld.db
DB += hiden_rga_degas.db
# BEGIN ANSIBLE MANAGED BLOCK
ifneq ($(RECCASTER),)
DB_INSTALLS += $(RECCASTER)/db/reccaster.db
endif
# END ANSIBLE MANAGED BLOCK

#----------------------------------------------------
# If <anyname>.db template is not named <anyname>*.template add
# <anyname>_TEMPLATE = <templatename>

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE

