# Leet_Code_Problem_Solving



# **Big O Notation - Interactive Guide**

Welcome to the **Big O Notation Interactive Guide**! 🚀

This repository provides **visual explanations** of **Big O complexity** using **HTML, CSS, and JavaScript**. Whether you're a beginner or an expert, this guide will help you understand how different algorithms scale.

---

## **📌 What is Big O Notation?**
Big O notation describes the **efficiency** of an algorithm in terms of **time complexity** and **space complexity**. It tells us how the performance changes as the input size (`n`) grows.

### **Common Complexities:**
| Notation | Complexity Type | Example Algorithm |
|----------|----------------|------------------|
| O(1)  | Constant Time  | Accessing an array element |
| O(log n) | Logarithmic Time | Binary search |
| O(n)  | Linear Time  | Loop through an array |
| O(n log n) | Linearithmic Time | Merge Sort, Quick Sort |
| O(n²) | Quadratic Time | Bubble Sort |

---

## **🎨 Live Visualization (HTML + CSS + JS)**
🎥 **Check out our interactive visualizations:** [Big O Playground](https://your-live-demo-link.com)

### **📄 How to Run Locally**
Clone this repository and open `index.html` in your browser:
```bash
git clone https://github.com/yourusername/big-o-visuals.git
cd big-o-visuals
open index.html
```

---

## **💡 Creative Implementations**

### **O(1) - Constant Time**
🔹 **Example:** Accessing an array index in JavaScript.
```js
const arr = [10, 20, 30];
console.log(arr[1]); // O(1)
```
🎨 **Visual:** Clicking a button retrieves a stored value instantly.

---

### **O(log n) - Logarithmic Time**
🔹 **Example:** Binary search in JavaScript.
```js
function binarySearch(arr, target) {
    let left = 0, right = arr.length - 1;
    while (left <= right) {
        let mid = Math.floor((left + right) / 2);
        if (arr[mid] === target) return mid;
        arr[mid] < target ? left = mid + 1 : right = mid - 1;
    }
    return -1;
}
```
🎨 **Visual:** A **tree animation** showing the search narrowing.

---

### **O(n) - Linear Time**
🔹 **Example:** Looping through an array.
```js
arr.forEach(item => console.log(item)); // O(n)
```
🎨 **Visual:** Progress bar filling up as the loop iterates.

---

### **O(n log n) - Linearithmic Time**
🔹 **Example:** Merge Sort.
```js
function mergeSort(arr) {
    if (arr.length < 2) return arr;
    let mid = Math.floor(arr.length / 2);
    return merge(mergeSort(arr.slice(0, mid)), mergeSort(arr.slice(mid)));
}
```
🎨 **Visual:** Blocks splitting and merging back into order.

---

### **O(n²) - Quadratic Time**
🔹 **Example:** Bubble Sort.
```js
function bubbleSort(arr) {
    for (let i = 0; i < arr.length; i++) {
        for (let j = 0; j < arr.length - i - 1; j++) {
            if (arr[j] > arr[j + 1]) {
                [arr[j], arr[j + 1]] = [arr[j + 1], arr[j]];
            }
        }
    }
    return arr;
}
```

