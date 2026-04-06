#include<stdio.h>

int global = 100;    // Global: visible everywhere

void demo()
{
    int local = 50;  // Local: visible only in demo()
    printf("Local = %d\n", local);
    printf("Global = %d\n", global);
}

int main()
{
    demo();
    printf("Global = %d\n", global);
    // printf("%d", local); // ERROR! local not visible he>
    return 0;
}
