# Fibonacci-series
Fibonacci series in c
#include <stdio.h>
int main() {
    int i, n, t1 = 0, t2 = 1, t3;
    printf("Enter the number of terms: ");
    scanf("%d", &n);
    printf("Fibonacci Series: ");

    for (i = 1; i <= n; i++) {
        printf("%d, ", t1);
        t3 = t1 + t2;
        t1 = t2;
        t2 = t3;
    }

    return 0;
}
/*OUTPUT:
Enter the number of terms: 10
Fibonacci Series: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34
*/
