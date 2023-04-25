# Lab 2


## Part 1
***
## Part 2

**Original Code**

  ```
  # static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
  ```
  
  
  **JUnit Testing**
  
  *Creates a failure inducing output*
  ```
  # @Test
  Public void testReversed(){
  
  int array = {1,2,4,5};
    int[] result = array.reversed();
  
  assertArrayEquals(array,result);
  
  }
  ```
  
**Corrected Code**

*The error of the code was that it wasnt properly reversing the array. In the fourth line the wrong code uses `arr[i] = newArray[arr.length-i-1]`, which is incorrect because arr is copying from the wrong array. It instead should the other way around, that way new array is copying from the inputed array*

  ```
  # static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
  ```
  
  
  
  
  **JUnit Testing**
  
  *Does not create a falure inducing output*
  
  ```
  # @Test
  public void testReversed(){
  
  int[] array = {1,2,3,4,5};
  int[] result = array.reversed();
  
  assertArrayEquals(array,result);
  
  }
  ```
***

#Part 3

*What I've learned durin lab 2 and 3, was know what a relative path, working directory, and absolute path. I learned how to determine what the absolute path will be the outcome of an working directory and relative path.*
