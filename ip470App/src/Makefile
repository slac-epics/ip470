# Makefile.Host
TOP = ../..
include $(TOP)/configure/CONFIG

 #----------------------------------------
 #  ADD MACRO DEFINITIONS AFTER THIS LINE
 #=============================
USR_CFLAGS += -DUSE_TYPED_RSET -DUSE_TYPED_DSET -DUSE_TYPED_DRVET

DBD += drvAvme470.dbd
DBD += devAvme470.dbd

INC += drvAvme470.h

# Source files (for depends target):
LIBSRCS += drvAvme470.c
LIBSRCS += devAvme470.c

# Link everything into a library:
LIBRARY_IOC_vxWorks = Avme470
LIBRARY_IOC_RTEMS   = Avme470
Avme470_LIBS += Ipac
Avme470_LIBS += xipIo

include $(TOP)/configure/RULES
