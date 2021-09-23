export ASIO_ROOT := "/home/jarrod/Dev/asio/asio"

CXX=g++
CXXFLAGS=-std=c++20 -Wall -Wextra -fno-inline -pthread -fcoroutines -I$(ASIO_ROOT)/include -g -DASIO_ENABLE_HANDLER_TRACKING
SOURCE=$(wildcard *.cpp)
PROGRAMS=$(SOURCE:.cpp=)
DSYM=$(SOURCE:.cpp=.dSYM)

all: $(PROGRAMS)

clean:
	rm -rf $(PROGRAMS) $(DSYM)
