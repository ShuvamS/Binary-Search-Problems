# Binary-Search-Problems
solved questions on binary search
<br>
// //binary search
// #include <bits/stdc++.h>
// using namespace std;
// int binarysearch(int arr[] ,int n,int target){
//     int start = 0;
//     int end = n-1;
//     int mid = (start + end)/2;
//     while(start<=end){
//         int element = arr[mid];
    
//     if(element == arr[mid]){
//         return mid;
//     }
//     else if(target < element ){
//         end = mid -1;
//     }
//     else{
//         start = mid + 1;
//     }
//     mid = (start + end) / 2;
// }
// return -1;
// }
// int main(){
//     int arr[] = {1,3,5,7,9,11,13};
//     int n = 7;
//     int target = 11;
    
//     int indexoftarget = binarysearch(arr,n,target);
//     if(indexoftarget == -1){
//         cout<<"target not found"<<endl;
//     }
//     else{
//         cout<<"target found at"<<indexoftarget<<endl;
//     }
//     return 0;
// }
//binary search using stl
// #include <bits/stdc++.h>
int
// using namespace std;
// int main(){
//     vector<int>v{1,2,3,4,5};
//     if(binary_search(v.begin(),v.end(),6)){
//         cout<<"found";
//     }
//     else{
//         cout<<"not found"<<endl;
//     }
// }
//find the first occurence of an element
// #include <bits/stdc++.h>
// using namespace std;
// int checkoccurence(int arr[],int n,int target){
//     int s= 0;
//     int e = n -1;
//     int m = s + (e-s)/2;
//     int ans = -1;
//     while(s<=e){
//         if(arr[m] == target){
//             ans = m;
//             e = m -1;
//         }
//         else if(arr[m]<target ){
//             s = m+1;
//         }
//         else if(arr[m] > target){
//             e = m -1;
//         }
//         m = s + (e-s)/2;
//     }
//     return ans;
// }
// int main(){
//     int arr[7] = {1,2,3,4,4,5,6};
//     int n = 7;
//     int target = 4;
//     int index = checkoccurence(arr,n,target);
//     if(index == -1){
//         cout<<"no occurence"<<endl;
//     }
//     else{
//         cout<<"index is present at"<<index<<" ";
//     }
// }
//find the last occurence of taregt
// #include <bits/stdc++.h>
// using namespace std;
// int binarysearch(int arr[],int n,int target){
//     int s = 0;
//     int e = n-1;
//     int m = s+(e-s)/2;
//     int ans = -1;
//     while(s<=e){
//         if(arr[m] == target){
//             ans = m;
//             s = s+1;
//         }
//         else if(arr[m] > target){
//             e = m -1;
//         }
//         else if(arr[m] < target){
//             s = s +1;
//         }
//         m = s+(e-s)/2;
//     }
//     return ans;
// }
// int main(){
//   int arr[7] = {1,2,4,4,4,5,6};
//   int n = 7;
//   int target = 4;
//   int index = binarysearch(arr,n,target);
//   if(index == -1){
//       cout<<"no index found"<<endl;
//   }
//   else{
//       cout<<"last index is at"<<index;
//   }
// }
//total number of occurence
// #include <bits/stdc++.h>
// using namespace std;
// int binsearch(int arr[],int n,int target){
//     int s= 0;
//     int e = n -1;
//     int m = s + (e-s)/2;
//     int ans = -1;
//     while(s<=e){
//         if(arr[m] == target){
//             ans = m;
//             e = m -1;
//         }
//         else if(arr[m]<target ){
//             s = m+1;
//         }
//         else if(arr[m] > target){
//             e = m -1;
//         }
//         m = s + (e-s)/2;
//     }
//     return ans;
// }
// int binarysearch(int arr[],int n,int target){
//     int s = 0;
//     int e = n-1;
//     int m = s+(e-s)/2;
//     int ans = -1;
//     while(s<=e){
//         if(arr[m] == target){
//             ans = m;
//             s = s+1;
//         }
//         else if(arr[m] > target){
//             e = m -1;
//         }
//         else if(arr[m] < target){
//             s = s +1;
//         }
//         m = s+(e-s)/2;
//     }
//     return ans;
// }
// int main(){
//   int arr[7] = {1,2,4,4,4,5,6};
//   int n = 7;
//   int target = 4;
//   int index = binarysearch(arr,n,target);
//   if(index == -1){
//       cout<<"no index found"<<endl;
//   }
//   else{
//       cout<<"last index is at"<<index<<endl;
//   }
//   int index1 = binsearch(arr,n,target);
//       if(index == -1){
//           cout<<"no first index"<<endl;
//       }
//       else{
//           cout<<"last index is at"<<index1<<endl;
//       }
//   int totalindex = index - index1 +1;
//   cout<<"total index is"<<totalindex;
// }
//find missing elements
// #include <bits/stdc++.h>
// using namespace std;
// int main(){
//     int arr[5] = {1,2,3,5,6};
//     int n = 5;
//     int sum = 0;
//     int sum2 = 0;
//     for(int i = 0; i<n; i++){
//         sum+=arr[i];
//     }
//     for(int i = 0; i<=n+1;i++){
//         sum2+=i;
//     }
//     int missing = sum2-sum;
//     cout<<missing;
// }
//peak element from a mountain array
// #include <bits/stdc++.h>
// using namespace std;
// int peakelement(int arr[],int n){
//     int s = 0;
//     int e = n-1;
//     int m = s+(e-s)/2;
//     while(s<e){
//         if(arr[m] <arr[m+1]){
//             s = m+1;
//         }
//         else{
//             e = m;
//         }
//         m = s+(e-s)/2;
//     }
//     return e;
// }
// int main(){
//     int arr[] = {0,7,8,9,10,2};
//     int n = 6;
//     int peak = peakelement(arr,n);
//     cout<<"the peak element is"<<peak;
// }
//find the sq root of a number using binary search
// #include <bits/stdc++.h>
// using namespace std;
// int findsqrt(int n){
//     int s = 0;
//     int e = n;
//     int m = s+(e-s)/2;
//     int ans =-1;
//     while(s<=e){
//         if(m*m == n){
//             return m;
//         }
//         else if(m*m > n){
//             e = m-1;
//         }
//         else{
//             ans = m;
//             s = m+1;
//         }
//         m = s+(e-s)/2;
//     }
//     return ans;
// }
// int main(){
//     int n;
//     cout<<"enter the number"<<endl;
//     cin>>n;

//     int sqroot = findsqrt(n);
//     cout<<"the sq root of the number is"<<sqroot;

//     double finalans = sqroot;
//     int precision;
//     cout<<"enter the number of floating digits you want precision of"<<endl;
//     cin>>precision;

//     double step = 0.1;
//     for(int i = 0; i<precision; i++){
//         for(double j=finalans ; j*j<=n; j=j+step){
//             finalans = j;
//         }
//         step = step/10;
//     }
//     cout<<finalans;
// }
//find missing element
// #include <bits/stdc++.h>
// using namespace std;
// int element(vector<int>v){
//     int s = 0;
//     int e = v.size()-1;
//     int m = s+(e-s)/2;
//     while(s<=e){
//         if(v[m] != m+1 && v[m-1] == m){
//             return m+1;
//         }
//         else if(v[m] != m+1){
//             e = m-1;
//         }
//         else{
//             s = m+1;
//         }
//         m = s+(e-s)/2;
//     }
//     return -1;
// }
// int main(){
//     vector<int>v{1,2,4,5,6};
//     int missing = element(v);
//     cout<<"missing element is"<<missing;
// }
//find target in 2d array using binary search
//#include <bits/stdc++.h>
// using namespace std;
// int search(int arr[][3],int n,int m,int target){
//     int s = 0;
//     int e = (n*m)-1;
//     int mid = s+(e-s)/2;
//     while(s<=e){
//         int rowindex = mid/m;
//         int colindex = mid%m;
//         int element = arr[rowindex][colindex];
//         if(element == target){
//             return true;
//         }
//         else if(element > target){
//             e= mid -1;
//         }
//         else{
//             s = mid+1;
//         }
//         mid = s+(e-s)/2; 
//     }
//     return false;
// }
// int main(){
//     int arr[3][3] = {{1,2,3},{4,5,6},{7,8,9}};
//     int n = 3;
//     int m = 3;
//     int target = 11;
//     bool found= search(arr,n,m,target);
//     if(found){
//         cout<<"the target is found"<<endl;
//     }
//     else{
//     cout<<"target not found"<<endl;
// }
// }
