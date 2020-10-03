SOURCE	:= Main.c Trace.c Branch_Predictor.c
CC	:= gcc
TARGET	:= Main
LINK	:= -lm
FLAGSETS := -D_FILE_OFFSET_BITS=64  

all: $(TARGET)

$(TARGET): $(SOURCE)
	$(CC) -o $(TARGET) $(FLAGSETS) $(SOURCE) $(LINK)

clean:
	rm -f $(TARGET)

debug: $(SOURCE)
	$(CC) -o $(TARGET) $(SOURCE)$(FLAGSETS)  $(LINK) -g
