#include <stdio.h>

int main() {
    int n, count = 0;

    
    printf("Enter the number of elements in the array: ");
    scanf("%d", &n);

    int array[n]; 

    
    printf("Enter the elements of the array:\n");
    for (int i = 0; i < n; i++) {
        scanf("%d", &array[i]);
    }

    
    for (int i = 0; i < n; i++) {
        if (array[i] < 0) {
            count++;
        }
    }


    printf("Total number of negative numbers in the array: %d\n", count);

    return 0;
}
