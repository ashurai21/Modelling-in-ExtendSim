# Modelling-in-ExtendSim

**Steps for creating a model in ExtendSim**

**Step-1**
Click on the ExtendSim software icon on your desktop to open up home page.

![Home page](https://user-images.githubusercontent.com/103962807/167256459-f1102bb8-bdca-4a8e-a765-9ee0dfc89be9.JPG)

**Step-2**

Click on File > New Model to open up ExtendSim Worksheet.

![Model home page](https://user-images.githubusercontent.com/103962807/167256548-bf24901b-5ef7-4e27-bd5a-1d279ef5f1fd.JPG)

**Step-3**

Click on Run > Simulation Setup 
Do the necessary changes in the values of End time, runs, and global time units as per your requirement.

![image](https://user-images.githubusercontent.com/103962807/167255833-5c78d7d4-8b37-4dca-b86d-e412c73235d5.png)

**Step-4**

Start making a model with the help of library blocks.

1. Click on Create block under Item (library).

![image](https://user-images.githubusercontent.com/103962807/167255900-16c536d0-13f1-4107-b14d-15300c449d05.png)

2. Select Queue block by right click on the end of create block (i.e., green square box).

![image](https://user-images.githubusercontent.com/103962807/167255953-153def88-531d-41a0-9026-aa10872f36e9.png)

3. Select Activity block again by right click on the end of the queue block (i.e., green square box).

![image](https://user-images.githubusercontent.com/103962807/167255972-fccb204c-cb4c-443c-80c1-75c2bc795f3e.png)

4. Repeat the above steps to add a queue block at the end of the activity block. 

![image](https://user-images.githubusercontent.com/103962807/167255989-d32cb0b7-2276-4f35-b19c-7c93f68fa99c.png)

5. Repeat the above steps to add the activity block at the end of the queue block. 

![image](https://user-images.githubusercontent.com/103962807/167256005-727f4203-8d8f-458a-9e69-044d5738f37f.png)

6. Repeat Step-4 and Step-5 depending upon the number of stations in the project. 

![image](https://user-images.githubusercontent.com/103962807/167256016-4ac89b66-8de9-434a-837f-9148f30787c7.png)

![image](https://user-images.githubusercontent.com/103962807/167256021-0cb03d43-418d-4ed3-90e1-2c3834cd47be.png)

7. Assuming three stations in this project, add the exit block by right click on the end of the activity block.

![image](https://user-images.githubusercontent.com/103962807/167256031-70eb0fd9-d05b-4910-abfe-f0f49663fc2f.png)

8. Rename all the stations in help blank just by double left click on the activity block. 

![image](https://user-images.githubusercontent.com/103962807/167256038-9769ae95-7007-4492-ba8f-29455e033ca2.png)

9. Under activity, the block provides the necessary inputs for all the stations based on project requirements.
Specify delay type and delay value.

![image](https://user-images.githubusercontent.com/103962807/167256057-4e1cc4a6-deae-4fe0-85be-58a6d08793bc.png)

10.	Run the simulation model by left-clicking on the Run tab and then Run Simulation to get the result.

![image](https://user-images.githubusercontent.com/103962807/167256070-fd29caab-0129-4c90-a411-4cae148d2aac.png)

11.	Determining cycle time statistics in ExtendSim with the help of simulation variable, set, and an information block. 
Adding set block just after queue block. Add simulation variable to the set block.

![image](https://user-images.githubusercontent.com/103962807/167256088-bd383c77-12bf-41b5-9775-57af14c1231c.png)

Double left-click on Set block 

![image](https://user-images.githubusercontent.com/103962807/167256095-2394ded8-63ec-4970-a799-bda9803e6f8a.png)

Left-click on none under property name, a dialog box will appear to add a new value attribute > Enter the attribute name (say Return) 

![image](https://user-images.githubusercontent.com/103962807/167256113-40be709a-794b-4b05-ac5d-8da50c9227c7.png)

![image](https://user-images.githubusercontent.com/103962807/167256118-6a5f265d-4994-4e68-bfa8-e83d657f9d84.png)

Now, just before exit add an information block. It is used to return cycle time statistics.

![image](https://user-images.githubusercontent.com/103962807/167256128-3c53f0a4-3415-4c95-8055-6ca75fcda9ad.png)

Double left-click on the information block, under the timing attribute change it to Return.

![image](https://user-images.githubusercontent.com/103962807/167256132-461253e0-bee4-4339-8d57-cb6dc515e6b7.png)

After running the simulation, it will display the cycle time statistics.

![image](https://user-images.githubusercontent.com/103962807/167256139-06197aac-67ee-4f36-86b9-db69a5e7a995.png)

![image](https://user-images.githubusercontent.com/103962807/167256143-9ea16729-28bc-4d44-81a1-acbcd09e7669.png)

12.	Add shift block by clicking shift-tab on Item library. A default window will pop up. 

![image](https://user-images.githubusercontent.com/103962807/167256151-85a240e3-7fa9-416b-8738-819178388998.png)

Make necessary changes based on shift working time. And update the shift in each activity and queue block based on station operational time.

![image](https://user-images.githubusercontent.com/103962807/167256159-80ca992a-a27b-481c-84ee-fcfa77aae2da.png)
