# Leetcode_TwoSum
Exercise 1 of the Problem of Leetcode

/**
 * Note: The returned array must be malloced, assume caller calls free().
 */
int* twoSum(int* nums, int numsSize, int target) {
    int *p = malloc(sizeof(int)*2);
    if(!p) {
        for(int i = 0; i < numSize-1; i++) {
            int temp = target - nums[i];
            for(int j = i+1; j < numSize; j++) {
                if(nums[j] == temp) {
                    p[0] = i;
                    p[1] = j;
                    return p;
                }
            }
        }
    }
    return NULL;
}
