HASING

*********************************
INTERFACE:
// Declaration: C++ supports multiple implementations, but we will be using
// std::unordered_map. Specify the data type of the keys and values.
unordered_map<int, int> hashMap;

// If you want to initialize it with some key value pairs, use the following syntax:
unordered_map<int, int> hashMap = {{1, 2}, {5, 3}, {7, 2}};

// Checking if a key exists: use the following syntax:
hashMap.find(1) != hashMap.end(); // true
hashMap.find(9) != hashMap.end(); // false

// Accessing a value given a key: use square brackets, similar to an array.
hashMap[5]; // 3

// Note: if you were to access a key that does not exist, it creates the key with a default value of 0.
hashMap[342]; // 0

// Adding or updating a key: use square brackets, similar to an array.
// If the key already exists, the value will be updated
hashMap[5] = 6;

// If the key doesnt exist yet, the key value pair will be inserted
hashMap[9] = 15;

// Deleting a key: use the .erase() method.
hashMap.erase(9);

// Get size
hashMap.size(); // 3

// Iterate over the key value pairs: use the following code.
// .first gets the key and .second gets the value.
for (auto const& pair: hashMap) {
    cout << pair.first << " " << pair.second << endl;
}
*********************************
POINTS:
-> used when we have to calculate the frequency
-> stored as key value pairs
-> searching sorting deleteing o(1)
-> to avoid collisions stored as linked list
