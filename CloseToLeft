#include <bits/stdc++.h>

using namespace std;


int closeToLeft(vector<int> A,int n, int target)
{
    int l = -1, r = n; 
    while (r - l > 1) {
        int mid = l + (r - l) / 2;

        if (target <= A[mid])
            r = mid;
        else
            l = mid;
    }

    return r;
}

int main()
{
    int n, k;
    cin>>n>>k;

    vector<int> input(n);
    for (int i = 0; i < n; i++)
       cin>>input[i];

    for (int i = 0; i < k; i++) {
        int num;
        cin>>num;

        cout<<closeToLeft(input, n, num + 1)<<endl;;
    }

    return 0;
}
