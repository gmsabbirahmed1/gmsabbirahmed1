#include <stdio.h>

int main() {
    double num1,num2;
    char o;

    printf("Enter a number\n");
    scanf("%lf", &num1);

    printf("Enter an operator\n");
    scanf(" %c", &o);

    printf("Enter a number\n");
    scanf("%lf", &num2);

    if (o == '+') {
        printf("%f", num1 + num2);
    } else if (o == '-') {
        printf("%f", num1 - num2);
    } else if (o == '/') {
        if (num2 != 0) {
            printf("%f", num1 / num2);
        } else {
            printf("Error: Division by zero\n");
        }
    } else if (o == '*') {
        printf("%f", num1 * num2);
    } else {
        printf("Invalid operation\n");
    }

    return 0;
}
