## Search an element in a 1D array using linear search

```bash
#include <stdio.h>

int main() {
    int n, key, i, found = 0;
    printf("Enter number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter elements:\n");
    for (i = 0; i < n; i++)
        scanf("%d", &arr[i]);

    printf("Enter element to search: ");
    scanf("%d", &key);

    for (i = 0; i < n; i++) {
        if (arr[i] == key) {
            printf("Element found at position %d\n", i);
            found = 1;
            break;
        }
    }
    if (!found)
        printf("Element not found.\n");
    return 0;
}
```
