 #include <stdio.h>
//#define size 3
int main()
{
  int a[2][2];
  int b[2][2];
  int c[2][2];
  int row, col;
  printf("enter the numbers in a  : \n");
  for(row=0;row<2;row++)
  {
      for(col=0;col<2;col++)
      {
          scanf("%d",&a[row][col]);
      }
  }
  printf("enter the numbers in b : \n");
  for(row=0;row<2;row++)
  {
      for(col=0;col<2;col++)
      {
          scanf("%d",&b[row][col]);
      }
  }

  for(row=0;row<2;row++)
  {
      for(col=0;col<2;col++)
      {
          c[row][col]=a[row][col]-b[row][col];
      }
  }
  printf("the diff of a-b = \n");
  for(row=0;row<2;row++)
  {
      for(col=0;col<2;col++)
      {
          printf("%d",c[row][col]);
      }
      printf("\n");
  }
  return 0;

}

