CXXFLAGS += -std=c++11
LDFLAGS = -pthread -lsfml-network -lsfml-graphics -lsfml-window -lsfml-system -lsfml-audio
SOURCES=$(shell find . -name "*.cpp")
OBJECTS=$(SOURCES:%.cpp=%.o)
TARGET=experiments.o
FIDOLIB=../../Fido/build/fido.a

.PHONY: all
all: $(TARGET)

$(TARGET): $(OBJECTS)
	$(LINK.cpp) $^ $(LOADLIBES) $(LDLIBS) $(FIDOLIB) -o $@ $(LDFLAGS)

.PHONY: clean
clean:
	rm -f $(TARGET) $(OBJECTS)
