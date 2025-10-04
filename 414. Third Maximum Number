class Solution {
public:
    int thirdMax(vector<int>& nums) {
        
        sort(nums.begin(),nums.end());
        if(nums.size() == 1) return nums[0];
        if(nums.size() == 2) return nums[1];
        int count = 0,j;
        for(j = nums.size()-1; j > 0; j--){
            if(nums[j] != nums[j-1]){
                count++;
            }
            if(count == 2){
                return nums[j-1];
            }
        }
        if(count != 2){
            return nums[nums.size()-1];
        }
        
        return nums[0];
    

    }
};
