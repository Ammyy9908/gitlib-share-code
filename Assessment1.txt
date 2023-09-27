def linear_search(arr, key):
    for i, val in enumerate(arr):
        if val == key:
            return i  # Return the index of the found element
    return -1  # Return -1 if the element is not found

if __name__ == "__main__":
    # Read the number of elements
    n = int(input())

    # Read the array elements
    arr = [int(input()) for _ in range(n)]

    # Read the key to search for
    key = int(input())

    # Perform the linear search
    result = linear_search(arr, key)

    if result == -1:
        print("Element not found")
    else:
        print(f"Element found at index: {result}")
