# Arrays-Codes

Q.1:Given an integer array A of size N and an integer B, you have to return the same array after rotating it B times towards the right.

public class Solution {
    public int[] solve(int[] A, int B) {
        int n=A.length;
        B=B%n;
       reverse(A,0,n-1);
       reverse(A,0,B-1);
        reverse(A,B,n-1);
        //int[] ans=rev2+rev3;
       return A;
        
    }

    public void reverse(int A[],int si,int ei)
    {
        while(si<ei){
        int temp=A[si];
        A[si]=A[ei];
        A[ei]=temp;
        si++;
        ei--;
    }
    //return A;
}
}
