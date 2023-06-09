# **Installing VSCode** 
1. Follow this [link](https://code.visualstudio.com/) in order to download and install VSCode 
![image](https://user-images.githubusercontent.com/127058698/230822340-064d2684-98c2-4f85-8a70-63ea5fdf86f8.png)
2. Select the OS affilated with your PC
![image](https://user-images.githubusercontent.com/127058698/230822141-fff239fb-bbcc-4e6e-a8b4-5aa5844db8f6.png)
3. Follow through with the installation 
![image](https://user-images.githubusercontent.com/127058698/230822608-128bf123-afc8-427e-810e-d2199d110a0d.png)
4. Launch VSCode, once here, you have successfully install VSCode  
![image](https://user-images.githubusercontent.com/127058698/230822701-1bda1b3b-4b0f-4cc5-8cb5-4ad369369d50.png)
--- 
# **Remotely Connecting**
1. Follow this [link](https://sdacs.ucsd.edu/~icc/index.php) to grab your couse-specific ID (we are going to need this for later) 
![image](https://user-images.githubusercontent.com/127058698/230832323-60a714cd-968c-4707-8354-08e4eaef111b.png)
2. While here, you are going to have to reset your password, follow this [guide](https://drive.google.com/file/d/17IDZn8Qq7Q0RkYMxdiIR0o6HJ3B5YqSW/view) if assistance is needed
3. Install [Git](https://gitforwindows.org/) and follow through with the installation, once done, your terminal should have the ability to use Git
![image](https://user-images.githubusercontent.com/127058698/230832688-3ec0acf5-ef28-45f6-9e2a-1abea9089655.png)
4. In the terminal, input this command, while replacing zz with the course-specific ID you acquired during step 1

`ssh cs15lsp23zz@ieng6.ucsd.edu`

5. The following command lines would return this, type yes in the input
> ssh cs15lsp23zz@ieng6.ucsd.edu
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])? 
6. You would then be asked to input a password (this should be the password you inputted when  you resetted your password in step 2
![image](https://user-images.githubusercontent.com/127058698/230833869-2625ffe8-5fcb-4539-bae4-36dbe899afad.png)
7. You are now remotely connected!

---
# **Trying Some Commands**
![image](https://user-images.githubusercontent.com/127058698/230834221-d2b078eb-dde8-449d-b886-946eaac25af7.png)
1. I used cat to print out the contents of my text file
2. Then I used pwd see what the current working path directory is
3. Using cd ~, it reseted the current working directory to the parent directory 
4. Then I used "cd OneDrive\Documents" jumping a directory to set the current working directory to my Documents directory

![image](https://user-images.githubusercontent.com/127058698/233588078-d3b2d2da-995f-4b4f-a543-c23b3b0fafbe.png)

The command cd .. allows the user to go back a directory 

![image](https://user-images.githubusercontent.com/127058698/233587257-3820f777-e6c0-4d37-9e1f-e00ef2f08f4b.png)

Messing around with the cat command, I found out that you can copy a text file and send it to another text file. 


