# Qick

#include <stdio.h>
#include <stdlib.h>

int compare(const void* a, const void* b) {
 return (*(int*)a - *(int*)b);
}

int main() {
 int v[] = {3,1,2,5,4}; 
int n; qsort(v, 5, sizeof(int), compare); 
for (n = 0; n < 5; n++) 
printf("%d ", v[n]); 
return 0;
}
