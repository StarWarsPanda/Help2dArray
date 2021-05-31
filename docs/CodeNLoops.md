##Basic Getting and Setting

```
int[][] exampleArr = 
{
	{1,2,3},
	{4,5,6},
	{7,8,9}
};

System.out.println(exampleArr[0][1]); //Prints "2"

exampleArr[0][1] = 1; //Changes the value at row 1 and column 0

System.out.println(exampleArr[0][1]); //Prints "1"
```

##Loops

Setting the array
```
int[][] exampleArr = new int[3][5];

for(int j = 0;j < exampleArr.length;j++)
{
	for(int i = 0;i < exampleArr[j].length;i++)
	{
		exampleArr[j][i] = j + 1 * i + 1; //Finds the product of the row and column, offset by one
	}
}
```
Printing the array
```
//Method that prints out the 2D array
void print2DArray(int[][] arr)
{
	for(int j = 0;j < arr.length;j++)
	{
		for(int i = 0;i < arr[j].length;i++)
		{
			System.out.print("[" + arr[j][i] + "]");
		}
		System.out.println(); //Just create a new line for the next column
	}
}
```
##Basic example
```
//Finds and prints out the amount of evens in a 2D array
int count = 0;

int[][] exampleArr = 
{
	{1,2,3},
	{4,5,6},
	{7,8,9}
};

for(int j = 0;j < exampleArr.length;j++)
{
	for(int i = 0;i < exampleArr[j].length;i++)
	{
		if(exampleArr[j][i]%2 == 0)
		{
			count++;
		}
	}
}

System.out.println(count); //In this example, the count will be four
```
