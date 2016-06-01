AM_CPPFLAGS = $(CXX11_FLAGS) -I../src -I../scream/code
AM_CPPFLAGS += $(GLIB_CFLAGS)
AM_CXXFLAGS = $(PICKY_CXXFLAGS)

LDADD = ../src/libsourdough.a -lpthread
LDADD += $(GLIB_LIBS)

bin_PROGRAMS = ScreamClient ScreamServer

ScreamClient_SOURCES = \
		ScreamClient.cc Packet.hh Packet.cc Timerfd.hh Timerfd.cc \
		../scream/code/ScreamTx.h ../scream/code/ScreamTx.cpp \
		../scream/code/RtpQueue.h ../scream/code/RtpQueue.cpp \
		../scream/code/VideoEnc.h ../scream/code/VideoEnc.cpp

ScreamServer_SOURCES = \
		ScreamServer.cc Packet.hh Packet.cc Timerfd.hh Timerfd.cc \
		../scream/code/ScreamRx.h ../scream/code/ScreamRx.cpp
