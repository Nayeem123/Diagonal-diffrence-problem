# Diagonal-diffrence-problem
Given a square matrix, calculate the absolute difference between the sums of its diagonals. 
Logic----

 public static int diagonalDifference(List<List<Integer>> arr,int n) {
    // Write your code here
    int d1=0,d2=0;
    for(int i=0;i<arr.size();i++)
    {
        for(int j=0;j<arr.get(i).size();j++)
        {
            if(i == j)
            d1+=arr.get(i).get(j);
            if(i==n-j-1)
            d2+=arr.get(i).get(j);
        }
    }
return Math.abs(d1 - d2);
}
