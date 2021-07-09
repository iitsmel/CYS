# Format String
### **Definition and Code Example**
In C language, when outputting a string, will use printf( "%d", intnumber).<br>
Those "%d", "%n" and" %p" are different output formats.
```
int main() {
    int leak;
    printf("leaking%n", &leak);
    printf("%d\n", leak);
}
```
<br>

### **Examples**
[CVE-2021-35331](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-35331)
