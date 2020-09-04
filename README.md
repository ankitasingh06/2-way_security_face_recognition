# 2-way_security_face_recognition_system

Hello reader!!

• Project Aim :- 2-way security system using face recognition system.

• Tools and Technology used:-
  1. Redhat Linux VM
      - Redhat VM and some basic Linux commands
  2. Python Programming Language
      -  OpenCV technology to enable vision to computer vision
  3. Anaconda Python Distributor
     -  Jupyter Notebook as IDE to run program
      
• Project Description :-
Project is capable to set up a 2-way security system, while login to the Redhat VM.When any user comes to login into the VM with their Username and Password, then here the user have to go one more security feature that is, first they have to clear first round by getting recognize their face to the trained model and then the 2nd step is to enter their username and Password.

When both the level gets pass, that user can eassily access their VM.

• Project Explanation :-
So, first of all we have to build our model and train it with the authorized user's face , with the help of OpenCV(cv2 module).

1. First we have to form a data set of images, collection of the images is required to train the machine for the required face.Whose face to be detected , we have to form data set for those faces so that machine know that face and trained itself successfully.

- For this we have to import cv2 module first.

![Screenshot (800)](https://user-images.githubusercontent.com/60088271/92269458-d671a800-ef01-11ea-90a2-0ed17abbd225.png)

- Then we start our camera and let our program to capture those faces(say 100 images).

In cv2, there is a function videocapture() , which is used to open our camera , which is linked/connected with the system. By default ,our webcamera of Laptop is assigned with value "0".

![Screenshot (801)](https://user-images.githubusercontent.com/60088271/92269517-f30de000-ef01-11ea-9d37-609936edb250.png)

- And hence our code will save that dataset to the specified location.Below is the Screenshot of the location and saved images.

![Screenshot (808)](https://user-images.githubusercontent.com/60088271/92269548-0325bf80-ef02-11ea-9487-e11c565d0aaa.png)

2. Now we have to train the model , with the help of dataset.

![Screenshot (804)](https://user-images.githubusercontent.com/60088271/92269638-3405f480-ef02-11ea-945a-0e99328ea031.png)

3. And after that, trick of the security comes->
Here I have used, very basic command of linux of "user authentication system".

As soon as admin create the user(say ankita user) with the help of "useradd" command
   *   "useradd ankita"
   * setup password for the user
    - "passwd ankita"
   * Lock the user
    - "usermod -L ankita"
    
![Screenshot (811)](https://user-images.githubusercontent.com/60088271/92269678-454f0100-ef02-11ea-907a-f75d3f60809d.png)
    
Now, here the 2-way security can be used---->

so that ,when user come to login into their system, first the user has to unlock their account by face recognition system and after unlocking , user can login with their username and password.

For unlocking, the command used is:-
- "usermod -U ankita"

![Screenshot (805)](https://user-images.githubusercontent.com/60088271/92269753-6b74a100-ef02-11ea-800f-d795bd729072.png)

![Screenshot (807)](https://user-images.githubusercontent.com/60088271/92269809-90691400-ef02-11ea-8848-a568c490a4d9.png)

4. After training with the model , now we have to check our model , so for testing we run following code and set the condition with the help of if-else statement, if the face gets detected with the accuracy greater or equl to 90% then, putText() that "Face Matched" and hence run the if block otherwise run else block.

>>Try-except block is also used, in case there is no face detected,except block will be executed.

![Screenshot (813)](https://user-images.githubusercontent.com/60088271/92271264-1c7c3b00-ef05-11ea-978c-c8a39ac0a366.png)

>> User comes to login into the system :-

![Screenshot (809)](https://user-images.githubusercontent.com/60088271/92269959-ca3a1a80-ef02-11ea-9cb8-7f3fc6a07d27.png)

>> Now , without approval of face recognition system, he/she cannot login, even though the user is entering right username and pasword :-

![Screenshot (812)](https://user-images.githubusercontent.com/60088271/92270131-1c7b3b80-ef03-11ea-9a32-87f7efd0c9c4.png)

>> As soon as the authorized user comes and , as soon as face gets matched, the if block will run and "usermod -U ankita" will get executed. So first round of security gets successfully completed and now when the user will come to login, He/she can login successfully. 

![Screenshot (821)](https://user-images.githubusercontent.com/60088271/92273473-0c665a80-ef09-11ea-9585-bc08be4db7e2.png)

![Screenshot (810)](https://user-images.githubusercontent.com/60088271/92270394-9c090a80-ef03-11ea-9c99-67d83cade3cc.png)

So this is how, our own developed "2-way security system" successfully worked.

⁕ you can also refer to the program code that has been attached to the repository.

Thank you

  
