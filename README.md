# algorithm  
 My Learning Process of Algorithms  
 record to practice algorithms problems.  
 leetcode_1 two-sum:  
 给定一个整数数组 nums 和一个目标值 target，请你在该数组中找出和为目标值的那两个整数，并返回他们的数组下标。  
 你可以假设每种输入只会对应一个答案。但是，你不能重复利用这个数组中同样的元素。  
 solution:  
 class Solution {  
    public int[] twoSum(int[] nums, int target) {  
        for (int i = 0; i < nums.length; i++) {  
            for (int j = i + 1; j < nums.length; j++) {  
                if (nums[j] == target - nums[i]) {  
                    return new int[] { i, j };  
                }  
            }  
        }  
        throw new IllegalArgumentException("没有相关值");  
    }  
}  
