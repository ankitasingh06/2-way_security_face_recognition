# 2-way_security_face_recognition_system

Hello reader!!

• Project Aim :- 2-way security system using face recognition system.

• Tools and Technology used:-
  1. Redhat Linux VM
      - RHEL8 VM and some basic Linux commands
  2. Python Programming Language
      -  OpenCV technology to enable vision to computer vision
  3. Anaconda Python Distributor
     -  Jupyter Notebook as IDE to run program
      
• Project Description :-
Project is capable to set up a 2-way security system, while login to the Redhat VM.When any user comes to login into the VM with their Username and Password, then here the user have to go one more security feature that is, first they have to clear first round by getting recognize their face to the trained model and then the 2nd step is to enter their username and Password.

When both the level gets pass, that user can eassily access their VM.

• Project Explanation :-
So, first of all weh have to build our model and train it with the authorized user's face , with the help of OpenCV(cv2 module).

And after that, trick of the security comes->
Here I have used, very basic command of linux of user authentication system.

As soon as admin create the user(say ankita user) with the help of "useradd" command
   *   "useradd ankita"
   * setup password for the user
    - "passwd ankita"
   * Lock the user
    - "usermod -L ankita"
    
Now, here the 2-way security can be used---->

when user come to login into their system, first they have to unlock their account by face recognition system and after unlocking , user can login with their username and password.

⁕ For better usnderstanding, Please refer to the program code that has been attached to the repository.

  
