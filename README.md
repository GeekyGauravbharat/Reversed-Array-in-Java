public class reversearray {
    
    public static void print(int arr[]) {
    for(int i = 0;i < arr.length;i++){
                System.out.print(arr[i]+" ");
        }
        System.out.println();
    }
     
    public static void main(String[] args) {
        int[] arr = { 2,3,4,6,13,14,17};
        print(arr);
        int n = arr.length;
        int i = 0 , j = n-1;
        while(i<j){
            int temp = arr[i];
            arr[i] = arr[j];
            arr[j] = temp;
            i++;
            j--;
        }
        print(arr);
    }
}// Reversed-Array
The basic approach to reverse an array is to iterate through the array and swap the elements of the array in such a way that it reverses the array, i.e., swap the first element with the last element, the second element with the second last element, and so on until we reach the middle of the array.
