# ReverseArrayProgram

import java.util.Arrays;
import java.util.Collections;

public class ReverseIntegerArray {
	public static void main(String[] args) {
		
		int [] arr = {1,2,3,4,5,6};
		
		System.out.println("Original Array: "+ Arrays.toString(arr));
		
		int[] reversedArr = Arrays.stream(arr)
		.boxed()
		.sorted(Collections.reverseOrder())
		.mapToInt(Integer::intValue)
		.toArray();
		
		System.out.println("Reversed Array: "+ Arrays.toString(reversedArr));
				
		
		
		
		
	}
	
}
