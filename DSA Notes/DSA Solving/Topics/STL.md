Iterators:
IT++->next location
and IT+1 ->next iterator

works both for vector and all
but not for maps
for example
vector<int>::iterator it;
auto->dynamically determines datatype
vector insertion and deletion ->o(1)
Map->access insertion LogN
for unordered->o(1)
m.clear()

multimap and multiset->allows duplicate values
ordered maps and sets take log n time 
unordered take o(1) insertion
find can be expensive 0(n) or o(log n)

Algorithms
accumulate->
sort->
upper_bound
lower_bound
(careful in maps and sets for above 2)
find->
count->
reverse->

Lambda functions:
[](int x){return x+2;}(4)

all_of(lambda function)