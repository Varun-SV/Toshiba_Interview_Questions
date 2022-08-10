# Toshiba_Interview_Questions
All Interview Questions from Toshiba with solutions
---
This is giithub repository having all the toshiba interview questions that the selected guys faced with the solutions.
---
## ***Participant 1***
Q1. Difference Betweeen the malloc and calloc?
*A1. We can differentiate the malloc and calloc on the basis of two different ways, one is syntactical and the other value initialization.*
> *For eg. if we want to create a integer array for 7 elements the following will be the syntactical difference : -*
 
```   int *arr,*arr2;
     int n,i;
     cout<<"Enter the number of elements : ";
     cin>>n;
     arr = (int *)malloc(n*sizeof(int));
     arr2 = (int *)calloc(n,sizeof(int));
     for(i=0;i<n-2;i++)
     {
          arr[i] = i+1;
          arr2[i]= i+1;
     }
     for(i=0;i<n;i++)
     {
          cout<<arr[i]<<" ";
     }
     cout<<endl;
     for(i=0;i<n;i++)
     {
          cout<<arr2[i]<<" ";
     }
     cout<<endl;
```
> *On running the code we will get the last two values in the **arr** to be a garbage value whereas in the **arr2** it will be assigned to '0'*<br>
> *The malloc only allocates the memory whereas the calloc allocates and initializes the values inside the array to zero.*
