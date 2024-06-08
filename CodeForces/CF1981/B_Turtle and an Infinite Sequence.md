Accepted Code:
```cpp
#include <bits/stdc++.h>
using namespace std;
int huo(int a,int b) {
	long long cnt = 0; 
        while(a != b) {
            cnt++;
            a >>= 1;
            b >>= 1;
        }
        while(cnt--) b = (b<<1)^1;
        return b;
}
int main() {
    int t; cin >> t;
    while(t--) {
    	int n,m; cin >> n >> m;
    	int l = max(n-m,0),r = n+m;
    	cout << huo(l,r) << endl;
    }
    return 0;
}
```
