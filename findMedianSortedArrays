    public static double findMedianSortedArrays(int[] nums1, int[] nums2) {
        int len3 = nums1.length +nums2.length;
        double median = 0;
        int[] nums3 = new int[len3];
        int i = 0, j = 0, k = 0;

        while (i < nums1.length && j < nums2.length) {
            if (nums1[i] <= nums2[j]) {
                nums3[k++] = nums1[i++];
            } else {
                nums3[k++] = nums2[j++];
            }
        }

        while (i < nums1.length) {
            nums3[k++] = nums1[i++];
        }

        while (j < nums2.length) {
            nums3[k++] = nums2[j++];
        }

        int half_len3 = len3/2;
        if(len3 % 2 == 0){
            median = (nums3[half_len3 - 1] + nums3[half_len3])/2.0;
        }else{
            median = nums3[half_len3];
        }
        return median;
    }
