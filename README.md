#include <stdio.h>

int sum_of_digits(int num) {
    int sum = 0;
    while (num != 0) {
        sum += num % 10;
        num /= 10;
    }
    return sum;
}

int main() {
    int a, b;
    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);
    
    int sum_a = sum_of_digits(a);
    int sum_b = sum_of_digits(b);
    
    printf("Sum of digits of %d is: %d\n", a, sum_a);
    printf("Sum of digits of %d is: %d\n", b, sum_b);
    
    return 0;
}
