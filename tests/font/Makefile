TARGET = fonttest
OBJS = fonttest.o ../../streams/streams.o ../../triVAlloc.o ../../triMemory.o ../../triRefcount.o ../../triImage.o ../../rle.o ../../triGraphics.o ../../triLog.o ../../triFont.o

INCDIR = 
CFLAGS = -O0 -G0 -Wall -g -DDEBUG -D_DEBUG -D_DEBUG_LOG -D_DEBUG_MEMORY -DTRI_SUPPORT_FT $(shell psp-pkgconf --cflags freetype2)
CXXFLAGS = $(CFLAGS) -fno-exceptions -fno-rtti
ASFLAGS = $(CFLAGS)

LIBS = -lpspgum -lpspgu -lpsprtc -lfreetype -lm -lz $(shell psp-pkgconf --libs freetype2)

BUILD_PRX = 1

EXTRA_TARGETS = EBOOT.PBP

all: clean

quick:

PSPSDK=$(shell psp-config --pspsdk-path)
include $(PSPSDK)/lib/build.mak
