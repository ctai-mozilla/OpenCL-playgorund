DEPTH = ../../../../..

include $(DEPTH)/make/openclsdkdefs.mk 

####
#
#  Targets
#
####

OPENCL			= 1
SAMPLE_EXE		= 1
EXE_TARGET 		= MemoryModel
EXE_TARGET_INSTALL   	= MemoryModel

####
#
#  C/CPP files
#
####

ifeq ($(OS), lnx) # Linux settings 
  ifeq ($(BITS), 64)
    C_RELEASE_FLAG    := -O2 -funswitch-loops -fgcse-after-reload -funroll-all-loops  -fexpensive-optimizations -ffast-math -finline-functions -frerun-loop-opt -static-libgcc
  endif
endif

FILES 	= MemoryModel
CLFILES	= MemoryModel.cl

include $(DEPTH)/make/openclsdkrules.mk 

