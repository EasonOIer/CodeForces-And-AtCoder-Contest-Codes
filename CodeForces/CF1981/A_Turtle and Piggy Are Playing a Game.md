Accepted Code:

```cpp
#include <bits/stdc++.h>
using namespace std;
int main() {
    int t; cin >> t;
    while(t--) {
    	int l,r; cin >> l >> r;
    	int x = 1,p = 0;
    	while(true) {
    		if((x >= l && x <= r) && !((x*2) >= l && (x*2) <= r)) break;
    		x *= 2;
    		p++;
    	}
    	cout << p << endl;
    }
    return 0;
}
```
