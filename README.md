# 🐍 Python Interview Preparation

> Complete Python interview prep — DSA patterns, system design, coding challenges & solutions

[![Stars](https://img.shields.io/github/stars/arya123224/python-interview-prep?style=for-the-badge&color=FFA116)](https://github.com/arya123224/python-interview-prep)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)

## 📚 Contents

### Data Structures
- Arrays & Strings
- Linked Lists
- Stacks & Queues
- Trees & Graphs
- Hash Maps
- Heaps & Priority Queues

### Algorithms
- Two Pointers
- Sliding Window
- Binary Search
- Dynamic Programming
- Backtracking
- Graph BFS/DFS

### Python Patterns
```python
# Two Pointers Pattern
def two_sum_sorted(nums, target):
    left, right = 0, len(nums) - 1
    while left < right:
        total = nums[left] + nums[right]
        if total == target: return [left, right]
        elif total < target: left += 1
        else: right -= 1
    return []

# Sliding Window Pattern
def max_subarray_sum(nums, k):
    window_sum = sum(nums[:k])
    max_sum = window_sum
    for i in range(k, len(nums)):
        window_sum += nums[i] - nums[i-k]
        max_sum = max(max_sum, window_sum)
    return max_sum

# Binary Search Pattern
def binary_search(nums, target):
    left, right = 0, len(nums) - 1
    while left <= right:
        mid = (left + right) // 2
        if nums[mid] == target: return mid
        elif nums[mid] < target: left = mid + 1
        else: right = mid - 1
    return -1
```

## ⭐ Star this repo if it helps you!

*By Harsh Kumar — github.com/arya123224*

