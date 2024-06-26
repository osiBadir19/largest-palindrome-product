#include <stdio.h>

int reverseInteger(int n) { 
// a function to find the reversal of the original number
    int reversal = 0;

    while (n > 0){
        reversal = reversal * 10 + n % 10;
        n = n / 10;
    }

    return reversal;
}

int main() {
    int n, reversal, max_n = 0, max_x1 = 0, max_x2 = 0;
    // iterate through 3 digits numbers
    for (int x1 = 100; x1 < 1000; x1++) {
        for (int x2 = 100; x2 < 1000; x2++) {
            // find the multiplication of the numbers
            n = x1 * x2;
            // find the reversal of the numbers
            reversal = reverseInteger(n);

            // if the reversal equals the origianl and the original is a new max then set variables to it
            if (n == reversal && n > max_n) {
                max_n = n;
                max_x1 = x1;
                max_x2 = x2;
            }
        }
    }

    printf("the max numbers are: %d and %d\n", max_x1, max_x2);
    printf("Their product is: %d\n", max_n);
    
    return 0;
}
