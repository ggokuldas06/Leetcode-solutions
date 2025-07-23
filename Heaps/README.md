HEAP interface in c++
->heaps are used when we want to repeatedly find maximum or minimum in a set of values
->does that in constant time
-> converts a vector to heap in constant time using iterators
*************************************************************************
// In C++, we will use std::priority_queue.
// By default, this implements a max heap
priority_queue<int> heap;

// Add to heap
heap.push(1);
heap.push(2);
heap.push(3);

// Check maximum element
heap.top(); // 3

// Pop maximum element
heap.pop();

// Get size
heap.size(); // 2

// Bonus: convert a vector into a heap in linear time
priority_queue<int> heap(nums.begin(), nums.end());
*************************************************************************
insertion o(n logn)
deletion O(n logn)
find min/max O(1)
*************************************************************************
top k elemetns with heap
{


'''vector<int> fn(vector<int>& arr, int k) {
    priority_queue<int, CRITERIA> heap;
    for (int num: arr) {
        heap.push(num);
        if (heap.size() > k) {
            heap.pop();
        }
    }

    vector<int> ans;
    while (heap.size() > 0) {
        ans.push_back(heap.top());
        heap.pop();
    }

    return ans;'''
}
*************************************************************************
