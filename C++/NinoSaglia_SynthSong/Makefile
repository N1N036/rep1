CXX = g++
CXXFLAGS = -Ic:/Program\ Files/JACK2/include -Wall -std=c++1z
LDFLAGS= -Lc:/Program\ Files/JACK2/lib32 -llibjack
SOURCE= osc.o sine.o wave.o adsr.o main.o jack_module.o 

example: $(SOURCE)
	$(CXX) -o $@ $(CXXFLAGS) $(SOURCE) $(LDFLAGS)

.cpp.o:
	$(CXX) -c $(CXXFLAGS) $<

clean:
	rm -f example *.o