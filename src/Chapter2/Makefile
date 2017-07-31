#** Start of PVCS Information ******************************
# $Archive:   //fnssnap1/pvcs/archives/Telepac/src/tools/scancards/Makefile-arc  $
# $Revision: 1.1.1.1 $
# $Modtime:   Aug 06 2002 14:52:56  $
# $Author: fnstpcd $
# $Date: 2006/12/25 03:36:11 $
#** End of PVCS Information ********************************

TAR1 = convert \ getinfo
OBJ1 = convert.cpp \ getinfo.cpp

TARGETS	= $(TAR1)
OBJECTS	= $(OBJ1)

MK_CMD_CPP=gcc
MK_FLG_CPP=-lstdc++
#
# Rules
#
.SUFFIXES: .cpp .obj .o
.cpp.obj:
	$(MK_CMD_CPP) $(MK_FLG_CPP) -o $@ -c $<
.cpp.o:
	$(MK_CMD_CPP) $(MK_FLG_CPP) -o $@ -c $<

#
# Targets
#

all: $(TARGETS)

$(TAR1): $(OBJ1)
	$(MK_CMD_BIN) $(MK_FLG_BIN) $(MK_FLG_OUT)$@ $(MK_LIB_PATH) $(OBJ1) $(MK_LNK_IFACE) $(MK_LNK_STAT)

clean: dirty
	rm -f $(OBJECTS) core

dirty:
	rm -f $(TARGETS)
