Source 1- Errichto Lectures

x<<i= x*2^k
2=2
0010=2

0100=2x2
1000=2x2x2
	   2x2^2
	   we shifted left by two places
x &(1<<i) and (x>>i)&1
represent same thing for digit
former is more intuitive but runs into long long issue

thats why people resort to second method but its no issue

Things to keep in mind
1.Swap
a^ a=0
so a^ a ^ b=b
Num1=(Num1^Num2); Num2=(Num1^Num2); Num1=(Num1^Num2);
2) Check If i’th bit is set or not: if((Num&(1<<i))!=0){ cout<<”SET”;} else{ cout<<”NOT SET”;} 3)
3) Set The i’th bit : Num=(Num|(1<<i)); 
4) Clear the i’th bit : Num=(Num&(~(1<<i))); 
5) Toggle the i’th bit : Num=(Num^(1<<i)); //toggles due to xor property
6) Remove the last set bit (RightMost) : Num=(Num&(Num-1));
7) Check power of 2: if((Num&(Num-1))==0){ cout<<”Power of 2”;} else{ cout<<”Not a power of 2”;} 
8) Check Number is odd or even : if((Num&1)==1){cout<<”odd”;} else {cout<<”even”;}
9) Divide a number by 2 : Num=(Num>>1);
10) Count number of set bits (C++ user) : int ans= __builtin_popcount(Num); 11) Count number of set bits (Other language) : int count=0; while(Num!=0){Num=(Num&(Num-1)); count++} return count;