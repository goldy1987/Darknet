# Darknet 
How to Install darknet in windows 10 system - No GPU


Step 1 : This is the most common step you will find in any tutorial. Clone Darknet git repo for windows by AlexeyAB.
          If you have git installed you can open command prompt and run command:
              
              git clone  https://github.com/AlexeyAB/darknet
              
   <img width="417" alt="1" src="https://user-images.githubusercontent.com/34401474/103397138-f423e680-4b5c-11eb-9894-f662fa4a65f5.PNG">
   
   If you don’t have git installed you can open above link and download zip and unzip (screen shot shared below)
   
   <img width="452" alt="2" src="https://user-images.githubusercontent.com/34401474/103397234-76140f80-4b5d-11eb-958c-2a7902143cbf.PNG">
   
Step 2: Open the Makefile in unzipped/downloaded folder darknet-master and change OPENCV=1 and save it.

   <img width="475" alt="3" src="https://user-images.githubusercontent.com/34401474/103397275-a6f44480-4b5d-11eb-96ee-28b2b8896b17.PNG">
    
Step 3: Go to 
          https://sourceforge.net/projects/opencvlibrary/files/opencv-win/3.3.0/opencv-3.3.0-vc14.exe/download  
and Download OpenCV
Create a folder named opencv_3.0 in C drive, double click the .exe file downloaded and unzip it in opencv_3.0 folder.
          
   <img width="364" alt="4" src="https://user-images.githubusercontent.com/34401474/103397299-c7240380-4b5d-11eb-8ccf-4d6f69f0fb70.PNG">
          
After this step add following path to Environment  Variables (Just for sanity check, copy these paths from your system.)
                    
                    C:\opencv_3.0\opencv\build\include 
                    C:\opencv_3.0\opencv\build\x64\vc14\lib
                    C:\opencv_3.0\opencv\build\x64\vc14\bin
                    
   <img width="302" alt="5" src="https://user-images.githubusercontent.com/34401474/103397334-f470b180-4b5d-11eb-8a26-72c9b701ba07.PNG">

Step 4: Download and Install Microsoft Visual Studio Community Edition 2019 from following link:
			
                              https://visualstudio.microsoft.com/
                              
   <img width="454" alt="6" src="https://user-images.githubusercontent.com/34401474/103397353-081c1800-4b5e-11eb-83b8-90b749e91aec.PNG">

Select Python development and Desktop development with C++ package too.

   <img width="453" alt="7" src="https://user-images.githubusercontent.com/34401474/103397389-326dd580-4b5e-11eb-8515-1fda902cd5dc.PNG">

Now this will take a while to finish Installing and it will take quit some Gigs on C Drive. To save some space in C Drive, go to Installation location and you can select different Drive for top two options: You can see in below I have changed path to G drive.
         
   <img width="454" alt="8" src="https://user-images.githubusercontent.com/34401474/103398008-b88b1b80-4b60-11eb-8139-2816f58d1397.PNG">

Step 5: Go to Darknet\build\darknet open darknet_no_gpu.sln file with Visual Studio
When you open, Visual Studio will ask to download two more dependencies allow it. This will take a little more time to complete. 

   <img width="455" alt="9" src="https://user-images.githubusercontent.com/34401474/103397407-49142c80-4b5e-11eb-9976-f486e74d1d0c.PNG">


Change Debug option to Release

   <img width="453" alt="10" src="https://user-images.githubusercontent.com/34401474/103397451-7a8cf800-4b5e-11eb-8a5e-a0476b7738ff.PNG">


Then click the .sln file once in Solution Explorer window so that it is selected (make sure it is collapsed)

   <img width="240" alt="11" src="https://user-images.githubusercontent.com/34401474/103397479-909ab880-4b5e-11eb-81ec-747fc6dab6cc.PNG">


Next go to Build option and click Build darknet_no_gpu

   <img width="454" alt="12" src="https://user-images.githubusercontent.com/34401474/103397495-aa3c0000-4b5e-11eb-884f-ebe5e3f5ffa9.PNG">

Process will end showing following message: 

========== Build: 1 succeeded, 0 failed, 0 up-to-date, 0 skipped ==========


Step 6: Now go to darknet\build\darknet\x64 folder and you will see darknet_no_gpu.exe has been created.
          <img width="357" alt="13" src="https://user-images.githubusercontent.com/34401474/103397524-c6d83800-4b5e-11eb-8d82-de57e6cf2fe3.PNG">

If you have successfully completed till this point. Congratulations have successfully installed Darknet in your Windows 10 system.

