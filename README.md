# array
#include <stdio.h>

int main(){
    // 1D array example
    int a;
    printf("enter the size of the array :");
    scanf("%d",&a);
    int arr[a];
    printf("enter %d elements for the 1D array\n",a);
    for(int i=0;i<a;i++){
        printf("enter=");
        scanf("%d",&arr[i]);
    }
     printf("\nElements of the 1D array are:\n");
    for(int i=0;i<a;i++){
        printf("%d\n",arr[i]);
    }
     // 2D array example
    int b,c;
    printf("\nEnter the number of rows and columns for the 2D array:\n");
    scanf("%d %d", &b, &c);

    int arr2[b][c];

    // Input elements for 2D array
    printf("Enter elements for the 2D array:\n");
    for (int i = 0; i < b; i++) {
        for (int j = 0; j < c; j++) {
            printf("Element at [%d][%d]: ", i + 1, j + 1);
            scanf("%d", &arr2[i][j]);
        }
    }

    // Display elements of 2D array
    printf("\nElements of the 2D array are:\n");
    for (int i = 0; i < b; i++) {
        for (int j = 0; j < c; j++) {
            printf("%d ", arr2[i][j]);
        }
        printf("\n");
    }

    return 0;
}
