# Event Ticket Inventory Engine (Python 3 + DSA)

A command-line ticket inventory management utility written in **Python 3**. This project combines core Python data structures (lists of dictionaries) with fundamental computer science algorithms (**Bubble Sort** and **Binary Search**) to organize and query event seating records efficiently.

---

## Algorithmic Complexity & Architecture
- **Data Representation:** Stores event records as a dynamic Python `list` of `dict` objects containing ticket codes, event names, and float pricing.
- **Bubble Sort (`bubble_sort_tickets`):**
  - **Mechanism:** Iteratively steps through the inventory list, compares adjacent ticket codes, and swaps unordered elements in-place using Python tuple unpacking (`a, b = b, a`).
  - **Time Complexity:** $O(n^2)$ worst-case and average-case complexity; $O(1)$ auxiliary space complexity.
- **Binary Search (`binary_search_ticket`):**
  - **Mechanism:** Requires a sorted collection. Repeatedly divides the search interval in half using integer floor division (`//`) to locate a target ticket code without scanning every record.
  - **Time Complexity:** $O(\log n)$ logarithmic time complexity—dramatically faster than $O(n)$ Linear Search for large datasets.

---

## How to Run Locally
1. Ensure **Python 3.10+** is installed on your system:
   ```bash
   python --version

#Clone this repository and navigate into the project directory:
          git clone [https://github.com/](https://github.com/)[your-github-username]/python-dsa-inventory.git
          cd python-dsa-inventory

#Execute the script in your terminal:
                                    python inventory_dsa.py