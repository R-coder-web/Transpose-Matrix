# Transpose-Matrix
#include <stdio.h>
int main(){
int a[10][10],transpose[10][10],n,i,j,row,col;
//take the row and column number from the user:
printf("enter your row amd colunm number: ");
scanf("%d %d",&row,&col);
//take the value of raw and column from user:

for(i=0;i<row;i++){

printf("\n");
for(j=0;j<col;j++){
        printf("a[%d][%d]: ",i,j);
scanf("%d",&a[i][j]);
}
}
//print the value of A matrix:
printf("\n");
printf("Matrix A: ");
for(i=0;i<row;i++){
printf("\n");
printf("\t");
for(j=0;j<col;j++){
printf(" %d",a[i][j]);
}
}
//make the transpose matrix:
printf("\n");

for(i=0;i<row;i++){
    printf("\n");
    
    for(j=0;j<col;j++){
        transpose[j][i]=a[i][j];

    }
}
//print the transpose matrix:
printf("\n");
printf("Transpose MAtrix: ");
for(i=0;i<col;i++){     /*because in transpose matrix raw would be column of any matrix:*/
    printf("\n");
    printf("\t");
    for(j=0;j<row;j++){
        printf("%d ",transpose[i][j]);
    }
}

}
