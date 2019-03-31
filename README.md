# Demo
package array;
import org.junit.Test;
public class array2 {
	public static void main(String args[]) {
		System.out.println("输出的子数组最大值为");
		int arca[] = { -1,3,2,-1,4 };			
		System.out.println(max(arca, 5));			
		};	
	 static int  max(int array[], int n)
		{
			int max = array[0], cur = 0;
			for (int i = 0; i < n; i++)
			{
				if (cur < 0)
				{
					cur = array[i];
				}
				else
					cur += array[i];
			}
			if (cur >= max)
			{
				max = cur;
			}
			return max;
		}
}



