#include<stdio.h>
#include<stdlib.h>

void TaoMang2Chieu(int ***a, int n, int m) {
	*a = (int**)malloc(n * sizeof(int*));
	for (int i = 0; i < n; i++) {
		(*a)[i] = (int*)malloc(m * sizeof(int));
	}
	for (int i = 0; i < n; i++) {
		for (int j = 0; j < m; j++) {
			printf("Nhap a[%d][%d]: ", i, j);
			scanf_s("%d", &(*a)[i][j]);
		}
	}
}

void XuatMang(int **a, int n, int m) {
	printf("Ma tran cua ban: \n");
	for (int i = 0; i < n; i++) {
		for (int j = 0; j < m; j++) {
			printf("%d", a[i][j]);
		}
		printf("\n");
	}
}

int main() {
	int** a;
	int n, m;
	printf("Nhap lan luot n va m: ");
	scanf_s("%d%d", &n, &m);
	TaoMang2Chieu(&a, n, m);
	XuatMang(a, n, m);
	for (int i = 0; i < n; i++) {
		free(a[i]);	
	}
	free(a);
	return 0;
}
