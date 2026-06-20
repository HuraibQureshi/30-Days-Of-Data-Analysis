# Day 1: Python Fundamentals for Analytics

Today, I focused on the vital structural primitives required to parse incoming raw data files before loading them into analytical engines.

### Key Learnings
1. **Dictionaries:** Excellent for handling incoming unstructured JSON data.
2. **List Comprehensions:** Fast, clean single-line looping for parsing and cleaning metrics.

### Code Snippet Executed
```python
# Raw transaction payload data data
raw_transactions = [
    {"user": "Alice", "amount": 150.50, "status": "completed"},
    {"user": "Bob", "amount": 240.00, "status": "pending"},
    {"user": "Charlie", "amount": 89.99, "status": "completed"}
]

# Using a list comprehension to filter completed data instantly
completed_orders = [tx for tx in raw_transactions if tx["status"] == "completed"]
print(f"Filtered Successful Logged Transactions: {completed_orders}")
