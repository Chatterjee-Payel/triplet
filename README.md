# triplet
          class Solution{
  public:
    //Function to find triplets with zero sum.
    bool findTriplets(int arr[], int n)
    { 
        //Your code here
        sort(arr,arr+n);
        int j,k,sum=INT_MAX;
        int i=0;
        for(int i=0;i<n-2;i++){
             int j=i+1;
        int k=n-1;
           while(j<k){
           sum=arr[i]+arr[j]+arr[k];
           {
            if(sum==0)
            {
             return 1;
        }
    else if(sum<0)
       {
           j++;
        }
                   else{
                       k--;
                   }
           }
 }
       }
         return 0;
    }
};
