### Quick Sort in C

```
void swap_r(int r[], int a, int b) {
    int temp = r[a];
    r[a] = r[b];
    r[b] = temp;
}
 
void quick(int r[], int start, int end) {
    if(end > start) {
        int pivot_index = (start + end) / 2;
        int pivot = r[pivot_index];
        int chg, i;
 
        swap_r(r, pivot_index, end);
 
        for(i = chg = start; i < end; i++) {
            if(r[i] < pivot) {
                swap_r(r, i, chg);
                chg++;
            }
        }
 
        swap_r(r, chg, end);
 
        quick(r, start, chg - 1);
        quick(r, chg + 1, end);
    }
}
```
