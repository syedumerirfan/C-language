# C-language (Code for Pyramid)
This is an assignment of Imperative programming of Computer Science of ELTE Class of 2024.
/* c code for a Pyramid */
#include <stdio.h>

int main()
{
    int n, i, j;
    printf("how many rows you want in pyramid?\n");
    scanf("%d", &n);
    for(i=1; i<=n; i++) 
    {
        
        for(j=1; j<=2*n-1; j++) 
        {
            
            if(j >= n-(i-1) && j <= n+(i-1))
            {
                printf("*");
            }
            else
                printf(" ");
        }
    printf ("\n");
    }
    return 0;
}

/* C-code for half pyramid */

#include <stdio.h>

int main()
{
    int n, i, j;
    printf("how many rows you want in half pyramid?\n");
    scanf("%d", &n);
    for(i=1; i<=n; i++) 
    {
        
        for(j=1; j<=i; j++) 
        {
                printf("*");
        }
    printf ("\n");
    }
    return 0;
}
