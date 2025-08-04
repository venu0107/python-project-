def list_operations():
    print("----- LIST OPERATORS & METHODS DEMO -----\n")

    # Create sample lists
    list1 = [1, 2, 3]
    list2 = [4, 5, 6]
    print(f"List 1: {list1}")
    print(f"List 2: {list2}\n")

    # Concatenation (+)
    combined = list1 + list2
    print(f"Concatenation (list1 + list2): {combined}")

    # Repetition (*)
    repeated = list1 * 2
    print(f"Repetition (list1 * 2): {repeated}")

    # Membership (in)
    print(f"Is 2 in list1? {'Yes' if 2 in list1 else 'No'}")

    # Length
    print(f"Length of list2: {len(list2)}")

    # Indexing
    print(f"First item of combined list: {combined[0]}")

    # Slicing
    print(f"Slicing combined[2:5]: {combined[2:5]}\n")

    # Append
    combined.append(7)
    print(f"After append(7): {combined}")

    # Insert
    combined.insert(2, 99)
    print(f"After insert(2, 99): {combined}")

    # Remove
    combined.remove(99)
    print(f"After remove(99): {combined}")

    # Pop
    popped = combined.pop()
    print(f"After pop(): {combined} (Popped: {popped})")

    # Sort
    combined.sort()
    print(f"After sort(): {combined}")

    # Reverse
    combined.reverse()
    print(f"After reverse(): {combined}")

    # Clear
    combined.clear()
    print(f"After clear(): {combined} (Empty list)")

if __name__ == "__main__":
    list_operations()
