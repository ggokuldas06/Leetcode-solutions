HEAP interface in c++
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
