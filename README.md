1. Compile file
```
as -o fileName.o fileName.s
```
2. Craete binary file
```
ld -o programe/FileName FileName.o \
    -lSystem \
    -syslibroot $(xcrun -sdk macosx --show-sdk-path) \
    -e _start \
    -arch arm64
```
3. Execute binary file
```
programe/HelloWorld
```