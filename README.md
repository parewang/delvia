def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        swapped = False
        for j in range(0, n-i-1):
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]  # Swap
                swapped = True
                print(f'Swap: {arr[j]} <-> {arr[j+1]} -> {arr}')
        if not swapped:
            break
    return arr

# Contoh penggunaan
numbers = [84, 54, 27, 16, 66, 13, 20]
print("Array sebelum diurutkan:", numbers)
sorted_numbers = bubble_sort(numbers)
print("Array setelah diurutkan:", sorted_numbers)

output dari program tersebut yaitu:
Array sebelum diurutkan: [84, 54, 27, 16, 66, 13, 20]
Swap: 54 <-> 84 -> [54, 84, 27, 16, 66, 13, 20]
Swap: 27 <-> 84 -> [54, 27, 84, 16, 66, 13, 20]
Swap: 16 <-> 84 -> [54, 27, 16, 84, 66, 13, 20]
Swap: 66 <-> 84 -> [54, 27, 16, 66, 84, 13, 20]
Swap: 13 <-> 84 -> [54, 27, 16, 66, 13, 84, 20]
Swap: 20 <-> 84 -> [54, 27, 16, 66, 13, 20, 84]
Swap: 27 <-> 54 -> [27, 54, 16, 66, 13, 20, 84]
Swap: 16 <-> 54 -> [27, 16, 54, 66, 13, 20, 84]
Swap: 13 <-> 66 -> [27, 16, 54, 13, 66, 20, 84]
Swap: 20 <-> 66 -> [27, 16, 54, 13, 20, 66, 84]
Swap: 16 <-> 27 -> [16, 27, 54, 13, 20, 66, 84]
Swap: 13 <-> 54 -> [16, 27, 13, 54, 20, 66, 84]
Swap: 20 <-> 54 -> [16, 27, 13, 20, 54, 66, 84]
Swap: 13 <-> 27 -> [16, 13, 27, 20, 54, 66, 84]
Swap: 20 <-> 27 -> [16, 13, 20, 27, 54, 66, 84]
Swap: 13 <-> 16 -> [13, 16, 20, 27, 54, 66, 84]
Array setelah diurutkan: [13, 16, 20, 27, 54, 66, 84]

