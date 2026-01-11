1.Set Matrix Zeroes
-Takeaway points
If you try to change and assign 0 midway it will change whole matrix
Use sets or vecs to store indices and based on indices you turn mat 0 the rigt way

to do inplace use first row,first column but since they collide at 0,0 we declare a column variable and traberse 0->0 for rows and col check like sets and then i-1 j=1 for iner matrix and then icheck first row and first col conditions and sorted.
2.Sort colours

Dutch Nation flagF->
low and mid at first high at end mid>=high
goal is low->0 mid->1 high->2 pointing to them

3.Next permutation

this one is tricky gotta revise

1 2 3
from 3 check smallest
1 3 2
then reverse at i+1->end also if bich mein v[j]>v[i] swap
if i<0 then reverse

just use stl next_permutation tbh

4.Majority Element

n/2 keep counter=1 reset to 0 again and counter+=1 again it shall reveal itself

5.4sum
Just move left and right pointers you can keep adding loops over og two sum problem to even do 5sum and 6sum etc....
sum<target l++ else r--; or both if sum reaches target

6.Best time to buy and sell stock 1 and 2

Use kadane's and greedy(ever increasing profit check from start keep moving start)

7.Subarray sum equals K
best question
mp[sum-k] it keeps track of prefix and we add mp[sum]++ why? because then we know if we had subtracted that sum from current prefix we would have got k

8.Encode and decode string

4#Neet
yeah do it like this
substr like i,j-i is len and then using that you could read and decode easily we will need to use both as one delmiter can be overridden

9.Top K frequenet 
use of map frequency and prirotiy queue to actually sort on the basis of the first value (inefficient waty would  be be putting map and custom sort)

10:Array wihtout that element in array
basically take prefix and postfix to check the sol prefix*postfix can even be done with variables without vectors

11.Longest consecutive
Clever set and hashmap traversal checking for succeeding /prev nums

12,Best buy sell stock 2-> ever increasing take minimum
13,Subarray sum equals K i mean dude if you have found sum-k

lets suppose 1 2 3
so we total sum is 6 and we already computed mp[0] sum beinf 1+2->mp[3]++
then we should be able mp[6-4]=mp[3] + the one we found
see hasmap makes things better

14.Container with most water dude see heights it should click you we can actually use two pointers you get one big height dabble on that and traverse the other side crazy right o(n) soln

15 Rain water
monotinc stack and building water subtracting min height left or ight

16.Nearby Duplicate
sliding window logic with set erasure


17. Longest Repeating char replacement

you really need to consider the maximum of the chars and check window len subtract and see its relevance with k
18. Permutation String Like my dude just use two maps or two hash tables to make your life easier and compare in the windows because yeah sorting is a bad idea real bad o(n) soln
19. Minimum Size Subarray sum: bro its ....classic sliding window question o(n)


20. Minimum window substring-> trust me this is a clever use of hashmap its easy to figure out sliding window logic reducing count to -1 and checking if count== 0 for others can help maintain the count. one hashmap is sufficient
21. Sliding window maximum gotta shift one by one the most clever solution to this is deque where we constantly maintain the num that is max in the window once we hit the window range i<=k, priority queue pair can be used as well where we remove left, one by one once we hit window range so we still have max at top in the range
22. K closest mean is a crazy question its not even doirect sliding window but it uses its concepts tbh think of it like bs and how we are using to eliminate the other windows and once l and r do meet we have found our window aka all elements must be the closestt u know or take the easier way out and sort this fella



