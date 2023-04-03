# Wake-on-LAN (WOL) is a network feature that allows a computer to be turned on or awakened from a low power state (S3) using a special network message called a WOL packet. When a computer is put into S3 state, the system is suspended and the network adapter is powered down into a D3 Hot state. WOL can be used to remotely wake up a computer from a sleeping state, without physically pressing the power button.

# It's worth noting that Windows 10 does not support WOL in S4 or S5 states. S4 is also known as Hybrid Shutdown or Fast Startup, which is a default setting in Windows 10 that allows for faster boot times by saving the kernel session to the disk. When a user chooses to shut down their computer, Windows 10 will save the kernel session to disk and then shut down, putting the computer in S4 state. In this state, the network adapter is not powered, and WOL is not possible. S5 is a classic shutdown state, similar to Windows 7.

# However, it's possible that the firmware and device may support WOL in S4 or S5, and in that case, Windows won't be involved in the process.

To Enable WakeOnLan 

>First We Need To Enable It From Device Manager

>Second We Need To Disable Fast Start-Up 


# 01 Enable WakeOnLan From Device Manager

1. Open Device Manager
>Press The Windows Key And X  

```
Win + X
```

![1](https://user-images.githubusercontent.com/94680549/228818684-46b49e43-9b0d-4e0d-ad1f-d8bddb2a2332.png)

2. Click On The Drop Down Arrow Next To Network Adapters Then Right Click On Your Ethernet Adapter And Select Properties

![2](https://user-images.githubusercontent.com/94680549/228819339-9df08fa1-5d46-4f00-8840-a9e0da452830.png)

![3](https://user-images.githubusercontent.com/94680549/228823264-e2ae2191-c8f4-45df-82ed-1348c1889da3.jpg)

3. In The Properties Go To Power Management

![5](https://user-images.githubusercontent.com/94680549/228820806-ba6b9ad3-f8eb-48de-bbe5-f97668b6c7e9.jpg)

4. Turn On Allow The Computer To Turn Off This Device To Save Power, Then Turn On Allow This Device To Wake The Computer, And Turn On Only Allow A Magic Packet To Wake The Computer 

![5](https://user-images.githubusercontent.com/94680549/228821317-6aef7cff-17f1-4fd3-88a3-b27d186ca99b.png)

5. Turn Off Allow The Computer To Turn Off This Device To Save Power

![4](https://user-images.githubusercontent.com/94680549/228833972-a863a60d-cea1-4738-862a-acdfca187927.png)

6. In The Properties Go To Advanced And Enable Wake On Magic Packet 

![6](https://user-images.githubusercontent.com/94680549/228821826-20c468b5-ceb2-4581-9de6-7a417c40db3c.jpg)

7. In Advanced Enable Wake On Pattern Match

![7](https://user-images.githubusercontent.com/94680549/228822081-64ea2e3c-019a-4450-9bc1-6c12c774c1c6.jpg)

8. Set The Value Of WOL & Shutdown Link Speed To 10 Mbps First

![8](https://user-images.githubusercontent.com/94680549/228822931-8b589697-e118-4f32-a57a-d4e08d04afb4.jpg)

# 02 Disable Fast Start-Up

1. Open Power Options
>Press The Windows Key And R
```
Win + R
```
>Type
```
powercfg.cpl
```

![anydesk00004](https://user-images.githubusercontent.com/94680549/228832922-641fc970-47be-4d8f-a538-ed0f37f43c20.png)

2. Click On Choose What The Power Buttons Do

![anydesk00001](https://user-images.githubusercontent.com/94680549/228832987-a7bcff9c-3517-4d77-8ec6-fd4281b6e7ae.png)

3. Click On Change Settings That Are Currently Unavailable

![anydesk00000](https://user-images.githubusercontent.com/94680549/228833300-58bf51f8-374c-4986-b2be-7e38783e756f.png)

4. Disable Turn On Fast Start-Up And Save Changes 

![anydesk00003](https://user-images.githubusercontent.com/94680549/228833579-834a006a-0b45-4723-9b96-1f3b2c198843.png)



