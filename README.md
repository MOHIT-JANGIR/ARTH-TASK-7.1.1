# ARTH-TASK-7.1.1
# Task Description 📄

# 🌀 7.1.1: Elasticity Task
# 🔅Integrating LVM with Hadoop and providing Elasticity to DataNode Storage


# SOLUTION :
# -->> Firstly i have created 10 gb ebs and i have created 2 volumes in the same way. 
![Screenshot 2020-11-02 19 26 03](https://user-images.githubusercontent.com/61896468/97876089-53be6b00-1d41-11eb-9b9d-e6b0e9b95d81.png)
# -->> Then i attached both volumes to my aws ec2 instance.
![Screenshot 2020-11-02 19 29 41](https://user-images.githubusercontent.com/61896468/97876452-e0692900-1d41-11eb-992b-33ae517a60b5.png)
# -->> To check all devices or hard disks , i have run fdisk -l and here my ebs volume is visible.
![2020-10-30 (1)](https://user-images.githubusercontent.com/61896468/97873325-79497580-1d3d-11eb-83a5-27b6d9f49107.png)
# -->> Istall lvm package.
![](https://miro.medium.com/max/875/1*cC3EvQj4IMF9JA51Ucta4w.png)


# -->> To use lvm,first i need to create a physical volume (pv) from this ebs And pvdisplay is to confirm it is created or not.
![2020-10-30 (2)](https://user-images.githubusercontent.com/61896468/97873331-7a7aa280-1d3d-11eb-818f-4b2c40880228.png)
# -->> Now i created a volume group (VG) and it has 10 gb.
![2020-10-30 (3)](https://user-images.githubusercontent.com/61896468/97873343-7e0e2980-1d3d-11eb-91dc-055d5802dc1d.png)
# -->> Now i created logical volume (LV) of 5 gb from this vg and it is available to use.
![2020-10-30 (4)](https://user-images.githubusercontent.com/61896468/97873346-7f3f5680-1d3d-11eb-9569-b9b7215b7e1d.png)

# Now lvm is like partition ,we can format it.

![](https://miro.medium.com/max/875/1*MTB6W0H3gmBRvuJv-J5jpg.png)

# Here i am mounting it to /dn2
![](https://miro.medium.com/max/875/1*fZgrSV1Blbx_0bFoIJwQoQ.png)
# 
![](https://user-images.githubusercontent.com/61896468/97841618-37540b80-1d0c-11eb-91a9-67b082972df0.png)


![image](https://user-images.githubusercontent.com/61896468/97879314-da754700-1d45-11eb-923e-a698d1b99ba8.png)
# -->> 
![2020-10-30 (7)](https://user-images.githubusercontent.com/61896468/97873353-823a4700-1d3d-11eb-9819-b348de8b3b0e.png)
![2020-10-30 (8)](https://user-images.githubusercontent.com/61896468/97873363-849ca100-1d3d-11eb-8aaa-75e4e81c6edd.png)
![2020-10-30 (9)](https://user-images.githubusercontent.com/61896468/97873366-85cdce00-1d3d-11eb-83f3-8c7dd1f63e1d.png)
![2020-10-30 (10)](https://user-images.githubusercontent.com/61896468/97873369-86fefb00-1d3d-11eb-9aea-299949fe560a.png)
![2020-10-30 (11)](https://user-images.githubusercontent.com/61896468/97873373-88302800-1d3d-11eb-9866-81ade3e264a2.png)
![Screenshot 2020-11-02 19 24 37](https://user-images.githubusercontent.com/61896468/97876082-515c1100-1d41-11eb-92c5-29b6ae614337.png)


