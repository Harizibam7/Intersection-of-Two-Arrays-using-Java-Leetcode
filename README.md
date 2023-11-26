# Intersection-of-Two-Arrays-using-Java-Leetcode

    import java.util.*;
    class Solution {
        public int[] intersection(int[] nums1, int[] nums2) {
            Set<Integer> set = new HashSet<>();
            Set<Integer> set1 = new HashSet<>();
            for(int num:nums1){
                set.add(num);
            }
            for(int num:nums2){
                if(set.contains(num)){
                     set1.add(num);
                }
            }
            int[] arr = new int[set1.size()];
            int i =0;
            for(int num: set1){
                arr[i] =num;
                i++;
            }
            return arr;
        }
    }
