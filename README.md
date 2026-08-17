# Day-8
My c language daily practice 
#include <stdio.h>

int main()
{
    int n, digit;
    int sum = 0;
    int count = 0;
    int even = 0;
    int odd = 0;

    printf("Enter a number: ");
    scanf("%d", &n);

    while (n > 0)
    {
        digit = n % 10;

        sum = sum + digit;
        count++;

        if (digit % 2 == 0)
        {
            even++;
        }
        else
        {
            odd++;
        }

        n = n / 10;
    }

    printf("Sum of digits = %d\n", sum);
    printf("Total digits = %d\n", count);
    printf("Even digits = %d\n", even);
    printf("Odd digits = %d\n", odd);

    return 0;
}
