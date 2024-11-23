public static double findMedianSortedArrays2(int[] nums1, int[] nums2) {
        int totalLength = nums1.length + nums2.length;
        int half = totalLength / 2;
        boolean isEven = totalLength % 2 == 0;

        int i = 0, j = 0, count = 0;
        int prev = 0, current = 0;

        while (i < nums1.length || j < nums2.length) {
            if (i < nums1.length && (j >= nums2.length || nums1[i] <= nums2[j])) {
                prev = current;
                current = nums1[i++];
            } else {
                prev = current;
                current = nums2[j++];
            }

            if (count == half) {
                return isEven ? (prev + current) / 2.0 : current;
            }
            count++;
        }
        return 0.0;
    }
