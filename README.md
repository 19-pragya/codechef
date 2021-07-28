#include<cstdio>
#include<cstring>
#include<cstdlib>
#include<cctype>

#include<cmath>
#include<iostream>
#include<fstream>
#include<cassert>
#include<string>
#include<vector>
#include<queue>
#include<map>
#include<algorithm>
#include<set>
#include<sstream>
#include<stack>
#include<cassert>

using namespace std;

#define MEM(a,b) memset(a,(b),sizeof(a))
#define MAX(a,b) ((a) > (b) ? (a) : (b))
#define MIN(a,b)  ((a) < (b) ? (a) : (b))
#define MP make_pair
#define pb push_back
#define inf 1000000000
#define   M 1000000007

#define maxl 10
#define maxt 50


typedef long long  LL;
typedef pair<LL,LL> pl;
typedef vector<int> vi;
typedef vector<string> vs;
typedef vector<double> vd;

using namespace std;

int main()
{
	int m,i,j,k,T,cs=0,t=0,a,b;
	int L,K;
	vi A;
	string X,Y;
	
	scanf("%d",&T);
	assert(T>=1 && T<=maxt);

	while(T--)
    {
        cin>>X>>Y;
        int ok=1;
        int l=X.size();
        assert((int)X.size()==(int)Y.size());
        for(i=0;i<l;i++)
        {
            assert( X[i]=='?' || (X[i]>='a' && X[i]<='z'));
            assert( Y[i]=='?' || (Y[i]>='a' && Y[i]<='z'));
            if(X[i]!='?' && Y[i]!='?' && X[i]!=Y[i]) ok=0;
        }
        if(ok)
            puts("Yes");
        else
            puts("No");


    }


	return 0;
}
