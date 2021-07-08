# Off-by-one Overflow
### **Definition and Example**
Off-by-one means

```
# include <stdio.h>

void offbyone(char *arg) {
    char buffer[10];
    int i = 0;

    for(i = 0; 10 >= i; i++) {
        buffer[i] = arg[i];
    }
}

int main(int argc, char **argv) {
    offbyone(argv[1])
}
```

The size of the buffer array is 10 bytes, which means there will be 10 bytes in memory reserved.<br>
The index starts at [0] so if one wants to use up 10 elements, the loop should be " 10 > i".<br>
for (i = 0;  10 > i; i++) executes 10 times.<br>
for (i = 0; 10 >= i; i++) executes 11 times.<br>
This kind of buffer overflow also appears in the CTF pwn section.<br>