class Solution {
public:
    int thirdMax(vector<int>& nums) {
        
        sort(nums.begin(),nums.end());
        if(nums.size() == 1) return nums[0];
        if(nums.size() == 2) return nums[1];
        int count = 0,j;
        for(j = nums.size()-1; j > 0; j--){
            if(nums[j] != nums1. Basics & Traversal (Warm-up)

Remove Duplicates from Sorted Array (26)

Remove Element (27)

Merge Sorted Array (88)

Move Zeroes (283)

Max Consecutive Ones (485)

Single Number (136)

🔹 2. Searching & Binary Search Variants

Search in Rotated Sorted Array (33)

Find First and Last Position of Element in Sorted Array (34)

Search Insert Position (35)

Find Minimum in Rotated Sorted Array (153)

Find Peak Element (162)

Peak Index in a Mountain Array (852)

🔹 3. Subarray / Subsequence

Maximum Subarray (Kadane’s) (53)

Best Time to Buy and Sell Stock (121)

Maximum Product Subarray (152)

Maximum Sum Circular Subarray (918)

Subarray Sum Equals K (560)

Minimum Size Subarray Sum (209)

Subarray Sums Divisible by K (974)

🔹 4. Hashing & Frequency

Two Sum (1)

Majority Element (169)

Top K Frequent Elements (347)

Contains Duplicate (217)

Contains Duplicate II (219)

First Missing Positive (41)

Find All Duplicates in an Array (442)

🔹 5. Sorting & Rearrangement

Sort Colors (Dutch National Flag) (75)

Find the Duplicate Number (287)

Find All Numbers Disappeared in an Array (448)

Missing Number (268)

First Missing Positive (41) (repeat, very important)

Wiggle Sort II (324)

🔹 6. Prefix / Suffix / Running Sum

Product of Array Except Self (238)

Find Pivot Index (724)

Range Sum Query – Immutable (303)

Range Sum Query 2D – Immutable (304)

Continuous Subarray Sum (523)

🔹 7. Sliding Window

Longest Substring Without Repeating Characters (3)

Minimum Window Substring (76)

Sliding Window Maximum (239)

Maximum Average Subarray I (643)

Max Consecutive Ones III (1004)

Longest Repeating Character Replacement (424)

🔹 8. Matrix Problems

Spiral Matrix (54)

Set Matrix Zeroes (73)

Word Search (79)

Search a 2D Matrix II (240)

Rotate Image (48)

Valid Sudoku (36)

🔹 9. Advanced / Hard

Trapping Rain Water (42)

Container With Most Water (11)

Largest Rectangle in Histogram (84)

Maximal Rectangle (85)

Longest Consecutive Sequence (128)

Candy (135)

⚡ Total = 65 problems

✅ Pattern Recap

Basics → Remove, merge, shift, duplicate handling.

Binary Search → Sorted + rotated arrays.

Subarray → Kadane, prefix, sliding window.

Hashing → Duplicates, missing, majority, freq counts.

Sorting / Rearrangement → Dutch flag, missing + extra.

Prefix/Suffix → Range queries, product except self.

Sliding Window → Longest/shortest subarray patterns.

Matrix → Traversals + modifications.

Hard → Water, histogram, rectangle, sequence.j-1]){
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
