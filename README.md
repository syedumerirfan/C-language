# C-language (Paterns of Pyramid)
This is an assignment of Imperative programming of Computer Science of ELTE Class of 2024.
/* c code for a Pyramid */
    *
   ***
  *****
 *******
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

code for inverted half pyramid.
****
***
**
*
int main()
{
  int n, i, j;
  printf("Enter the number of rows\n");
  scanf("%d",&n);

  for(i=n; i>0; i--)
  {
    for(j=i; j>=1; j--)
    {
      printf("*");
    }
    printf("\n");
  }
  
  code for inverted two half pyramids
    **** ****
     *** ***
      ** **
       * *
       
#include <stdio.h>

int main()
{
	int n;
	scanf("%d", &n);
	for (int i = n; i >= 1; i--)
	{
		for (int j = 1; j <= n; j++)
		{
			printf(" ");
		}
		for (int p = 1; p <= i; p++)
		{
			printf("*");
		}
		printf(" ");
		for (int q = 0; q <= i - 1; q++)
		{
			printf("*");
		}
		printf("\n");
		n++;
	}
	return 0;
}       
