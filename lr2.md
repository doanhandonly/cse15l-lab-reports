Part 1
=========
![image](https://user-images.githubusercontent.com/127058698/234172208-f923b933-dca7-4b8e-9a3d-0eab02e4545f.png)
__1)__ 

![image](https://user-images.githubusercontent.com/127058698/234172749-ec0c958b-f48b-4847-bc70-e8dd5880e6b7.png)

* The method being called here is `handRequest`
* The relevant arguments to this method is the data type URI, which in this case is 
  > localhost:4000/add-message?s=

  The values of any relevant fields of the class would be what is after the "="
* The values of any relevant fields only adds to the str field, resulting in lines and lines of string whenever the server runs

__2)__

![image](https://user-images.githubusercontent.com/127058698/234177913-85d51baf-323f-46ee-82a1-fbd1e54f7af7.png)

* The method being called here is `handRequest`
* The relevant arguments to this method is the data type URI, which in this case is 
  > localhost:4000/add-message?s=

  The values of any relevant fields of the class would be what is after the "="
* The values of any relevant fields only adds to the str field, resulting in lines and lines of string whenever the server runs

(essentially, the same things happen when I ran the two queries) 

Part 2
=========
__Failure Inducing Input:__



    public void testReverseInPlace() {
    
      int[] input2 = {1,2,3};
    
      ArrayExamples.reverseInPlace(input2);
    
      assertArrayEquals(new int[]{3,2,1}, input2);
    }

__Non-Failure Inducing Input:__

    public void testReverseInPlace() {
    
      int[] input1 = {3};
    
      ArrayExamples.reverseInPlace(input2);
    
      assertArrayEquals(new int[]{3}, input1);
    }
    
 __Failure Inducing Input Symptom:__
 ![image](https://user-images.githubusercontent.com/127058698/234182066-d3b1b0f2-bc1d-4103-94b4-bae8315c5f82.png)

 __Non-Failure Inducing Input Symptom:__
 
 ![image](https://user-images.githubusercontent.com/127058698/234181949-36d397e6-6121-4379-9e11-480ee42941a9.png)

__Before Code__



    static void reverseInPlace(int[] arr) {
      for(int i = 0; i < arr.length; i += 1) {
        arr[i] = arr[arr.length - i - 1];
      }
    }
    
__After Code__

    static void reverseInPlace(int[] arr) {
      for(int i = 0; i < arr.length / 2; i += 1) {
        arr[i] = arr[arr.length - i - 1];
        int temp = arr[i];
        arr[i] = arr[arr.length - i - 1]; 
        arr[arr.length - i - 1] = temp;
      }
    }
    
The issue was that once the array was changed in the first half, the original first half of the array was erased from existence and you could not get back the original first half values of the array. Adding a temporary variable helped store the first half of the array, and adding to the end of the array. 

Part 3
=========
In the most recent lab, lab 3, I learned that there are layers to debugging, and it is more sophiscated then just spending hours staring at a line of code. That there is a more effective approach to debugging then staring. Breaking down debugging, things you have to consider. These things are the failure-inducing input, the symptom (which is the output of the failure-inducing input / faulty behavior). And the bug itself (the thing that is causing programmers across the world nightmares). 

