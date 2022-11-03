libgomp-playground
==================

### Makefile
```
# Project: Project1
# Makefile created by Embarcadero Dev-C++ 6.3

CPP      = g++.exe
CC       = gcc.exe
WINDRES  = windres.exe
OBJ      = main.o
LINKOBJ  = main.o
LIBS     = -L"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/lib" -L"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/x86_64-w64-mingw32/lib" -static -lgomp
INCS     = -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/include" -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/x86_64-w64-mingw32/include" -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/lib/gcc/x86_64-w64-mingw32/9.2.0/include"
CXXINCS  = -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/include" -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/x86_64-w64-mingw32/include" -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/lib/gcc/x86_64-w64-mingw32/9.2.0/include" -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/lib/gcc/x86_64-w64-mingw32/9.2.0/include/c++"
BIN      = Project1.exe
CXXFLAGS = $(CXXINCS) -fopenmp
CFLAGS   = $(INCS) -fopenmp
DEL      = C:\Users\Administrator\Downloads\Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable\devcpp.exe INTERNAL_DEL

.PHONY: all all-before all-after clean clean-custom

all: all-before $(BIN) all-after

clean: clean-custom
	${DEL} $(OBJ) $(BIN)

$(BIN): $(OBJ)
	$(CPP) $(LINKOBJ) -o $(BIN) $(LIBS)

main.o: main.cpp
	$(CPP) -c main.cpp -o main.o $(CXXFLAGS)
```
