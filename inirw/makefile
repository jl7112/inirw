INC= 
LIBS= 

CFLAGS= -std=c++0x -g -Wall -Wno-deprecated

BIN= test
OBJECTS= inirw.o test.o
all: $(BIN)

%.o: %.cpp 
	@echo 
	@echo "Compiling $< ==> $@..." 
	$(CXX) $(INC) $(CFLAGS) -c $< -o $@ 
 
%.o: %.c 
	@echo 
	@echo "Compiling $< ==> $@..." 
	$(CC) $(INC) $(CFLAGS) -c $< -o $@

test: $(OBJECTS)
	@echo
	@echo "create archive $@...."
	$(CXX) -o $(BIN) $(OBJECTS) $(LIBS)

clean:
	rm -f $(BIN) 

