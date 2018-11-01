
'
class Solution {
    public int arrayPairSum(int[] nums) {
        //排序
        Arrays.sort(nums);
        //奇数加
        int sum = 0;
        for(int i = 0; i < nums.length/2; i+=2 ){
            sum+=nums[i];
            if(i == (nums.length-1)>>1)
                break;
            sum+=nums[nums.length-2-i];
        }        
        return sum;
    }
}
'
