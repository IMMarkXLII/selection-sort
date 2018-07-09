# selection-sort

```
  static void selectionSort(int arr[]) {
		int min = 0;
		for(int i = 0; i < arr.length - 1 ; i++) {
			min = i;
			for(int j = i+1; j<arr.length  ; j++) {
				if(arr[j] < arr[min]) { // for ascending order . for decending order change to arr[j] > arr[min]
					min = j;
				}
			}
			if(min != i) {
				int tmp = arr[min];
				arr[min] = arr[i];
				arr[i] = tmp;
			}
		}
	}
  
  ```
