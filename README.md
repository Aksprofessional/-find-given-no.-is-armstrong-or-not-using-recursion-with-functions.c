# -find-given-no.-is-armstrong-or-not-using-recursion-with-functions.c
// C program to find given no. is armstrong or not using recursion with functions.
// C program to find given no. is armstrong or not using recursion with functions

#include <stdio.h>
int arm(int);
int main() {
    int n,s;
    printf("enter no.=");
    scanf("%d",&n);
    s=arm(n);
    if(n==s)
        printf("armstrong no.");
    else
        printf(" not an armstrong no.");

    return 0;
}
int arm(int n){
    int r=n%10,s=0;
    if(n==0)
    return 0;
    return s+r*r*r+arm(n/10);
}
