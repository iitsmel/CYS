# Uninitialized Variable
### **Definition**
A variable's value is not defined before it is used.

<br>

### **Example**

A simple explanation.<br>

```
void uninitializedvariable() {
    int i, y;

    for(i = 0; 10 > i; i++) {
        y++;
    }

    printf("%d", y)
}
```

<br>

[CVE-2016-8385](https://www.cvedetails.com/cve/CVE-2016-8385/)