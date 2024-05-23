1
#include <stdio.h>

int main(void) {
    float var1, var2;
    printf("Enter the first number (var1): ");
    scanf_s("%f", &var1);
    printf("Enter the second number (var2): ");
    scanf_s("%f", &var2);
    printf("var1 > var2 is %d\n", var1 > var2);
    printf("var1 < var2 is %d\n", var1 < var2);
    printf("var1 == var2 is %d\n", var1 == var2);
    printf("var1 >= var2 is %d\n", var1 >= var2);
    printf("var1 <= var2 is %d\n", var1 <= var2);
    printf("var1 != var2 is %d\n", var1 != var2);
    int Ivar1 = var1, Ivar2 = var2; 
    printf("Ivar1 is %d\n", Ivar1);
    printf("Ivar2 is %d\n", Ivar2);
    printf("var1 || var2 is %d\n", var1 || var2);
    printf("var1 && var2 is %d\n", var1 && var2);

    return 0;
}
2
#include <stdio.h>

#define TRUE "TRUE"
#define FALSE "FALSE"

int main(void) {
    float var1, var2;
    printf("Enter the first number (var1): ");
    scanf_s("%f", &var1);
    printf("Enter the second number (var2): ");
    scanf_s("%f", &var2);
    printf("var1 > var2 is %s\n", var1 > var2 ? TRUE : FALSE);
    printf("var1 < var2 is %s\n", var1 < var2 ? TRUE : FALSE);
    printf("var1 == var2 is %s\n", var1 == var2 ? TRUE : FALSE);
    printf("var1 >= var2 is %s\n", var1 >= var2 ? TRUE : FALSE);
    printf("var1 <= var2 is %s\n", var1 <= var2 ? TRUE : FALSE);
    printf("var1 != var2 is %s\n", var1 != var2 ? TRUE : FALSE);
    int Ivar1 = (int)var1, Ivar2 = (int)var2; 
    printf("Ivar1 is %s\n", Ivar1 ? TRUE : FALSE);
    printf("Ivar2 is %s\n", Ivar2 ? TRUE : FALSE);

    printf("var1 || var2 is %s\n", var1 || var2 ? TRUE : FALSE);
    printf("var1 && var2 is %s\n", var1 && var2 ? TRUE : FALSE);

    return 0;
}
3
#include <stdio.h>
#include <conio.h>

int main() {
    int a = 0, b = 3, c; 
    c = b % 2 || (a >= 0) && (++b / (2 * a)) == 0;
    printf("a=%d, c=%d\n", a, c);
    _getch();
    return 0;
}
4
#include <stdio.h>#include <stdio.h>
#include <conio.h>

int main() {
    int a = 1, b = 0, c;
    c = (a >= 0) && (++b * a) == 0;
    printf("c=%d\n", c);
    _getch();
    return 0;
}
5
#include <stdio.h>
#include <conio.h>

int main() {
    int x = 1, y = 2, z;
    z = (x / 27 <= 0) && (y < 0) || (y % x == 0);
    printf("z=%d\n", --z);
    _getch();
    return 0;
}
6
#include <stdio.h>
#include <conio.h>

int main() {
    int x = 1, z, be = 0, y = 2;
    z = (x + y == 0) || be++ || (x / y * 3 == 0);
    printf("z=%d\n", z);
    _getch();
    return 0;
}
7
#include <stdio.h>
#include <conio.h>

int main() {
    int x = 2, z, y = 0;
    z = (x == 0) && (y = x) || (y > 0); 
    printf("z=%d\n", z);
    _getch();
    return 0;
}
8
#include <stdio.h>
#include <conio.h>

int main() {
    unsigned int x = 2, y = 1, z = 3;
    char chx = 0xAF;
    printf("%u\n", x & y & z);
    x = y = z = 2;
    printf("%u\n", x & y & z);
    x = 3;
    y = 0;
    z = 1;
    printf("x^y|~z=%u\n", x ^ y | ~z);
    _getch();
    return 0;
}
9
#include <stdio.h>
#include <conio.h>

int main() {
    char x = 255, y = 0177;
    printf("%u\n", (unsigned char)x & (unsigned char)y);
    x = '\0';
    y = 127;
    printf("%u\n", (unsigned char)x & (unsigned char)y);
    y = 128;
    printf("%u\n", (unsigned char)x & (unsigned char)y);
    _getch();
    return 0;
}
