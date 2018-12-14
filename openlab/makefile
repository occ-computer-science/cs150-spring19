EXE = app
CXX = @clang++
CXXFLAGS = -ggdb3 -O0 -std=c++14 -Wall -Wextra -Wshadow
SRC = $(EXE).cpp
OBJS = $(EXE).o

$(EXE): $(OBJS) makefile
	$(CXX) $(CXXLAGS) -o $@ $(OBJS)

# Remove object files from folder
clean:
	rm -f core $(EXE) *.o

test: $(EXE)
	@./$(EXE) test

run: $(EXE)
	@./$(EXE)
