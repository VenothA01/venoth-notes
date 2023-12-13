## topics_covered.md

-[ ] API
    - [ ] http methodss
            - GET
            - POST
            - PUT is idempotent
            - DELETE
            - OPTIONS
            - HEAD
    - [ ] data formats       



    search sorted arr


        - implement bs


N = arr.length;
start = 0;
end = N-1;

while(start <=end){

    int mid = start + end/2;


    if(arr[mid]==k)
        return ;
    else if(arr[mid]< k)
        start = mid+1;
    else
        end = mid -1;
        
}


4, 5, 1, 2, 3  

\       int left = 0;
        int right = arr.length - 1;

        while (left <= right) {
            int mid = (left + right) / 2;

            if (arr[mid] == target) {
                return mid; // Element found, return its index
            } else if (arr[left] <= arr[mid]) {
                // Left half is sorted
                if (arr[left] <= target && target <= arr[mid]) {
                    // Target is in the left half
                    right = mid - 1;
                } else {
                    // Target is in the right half
                    left = mid + 1;
                }
            } else {
                // Right half is sorted
                if (arr[mid] <= target && target <= arr[right]) {
                    // Target is in the right half
                    left = mid + 1;
                } else {
                    // Target is in the left half
                    right = mid - 1;
                }
            }
        }

        return -1; 