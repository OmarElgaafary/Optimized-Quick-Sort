#include <iostream>

void swap(int& a, int& b);
void printarr(int arr[], int length);
int QuickSortPartition(int arr[], int low, int high);
void QuickSort(int arr[], int low, int high);
void QuickSort(int arr[], int low, int high);





int main() {

	int data[10] = {5, 9, 3, 10, 8, 6, 1, 2, 7, 4};
	QuickSort(data, 0, 9);
	printarr(data, 10);
	

}

void swap(int& a, int& b) {
	int temp = a;
	a = b;
	b = temp;
}

void printarr(int arr[], int length) {
	std::cout << "[";
	for (int i = 0; i < length; i++) {
		std::cout << arr[i];
		if (i < length - 1) {
			std::cout << ", ";
		}
	}
	std::cout << "]";
}

int QuickSortPartition(int arr[], int low, int high) {

	int pivot = arr[high];
	int i = low - 1;
	for (int j = low; j < high; j++) {
		if (arr[j] <= pivot) {
			i++;
			swap(arr[i], arr[j]);
		}
	}
	i++;
	swap(arr[i], arr[high]);
	return i;
}

void QuickSort(int arr[], int low, int high) {
	if (low < high) {
		int pivot_point = QuickSortPartition(arr, low, high);
		QuickSort(arr, low, pivot_point - 1);
		QuickSort(arr, pivot_point + 1, high);

	}
}







