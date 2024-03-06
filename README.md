# Algoritimo-2
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        swapped = False
        for j in range(0, n-i-1):
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]
                swapped = True
        if not swapped:
            break
    return arr

vetor = [9,5,7,2,6,1,3,0,4,8]
print("Vetor original:", vetor)
print("Vetor ordenado:", bubble_sort(vetor))
