# Disable Feature Updates From The Registry

1.Open The Registry(regedit.exe)

>Press The Windows Key And R
```
Win+R
```
>Type regedit.exe
```
regedit.exe
```

![1](https://user-images.githubusercontent.com/94680549/228783149-084f4f3a-fe80-4e4b-8ae8-732f39dc23f9.png)

![2](https://user-images.githubusercontent.com/94680549/228783208-dc636ad8-01be-4502-b23f-db009fa15524.png)

2.Navigate To 
```
Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows
```

![3](https://user-images.githubusercontent.com/94680549/228784833-9b6fb226-9594-410a-86f1-7dfe29deed7a.png)

3.Right Click On The Key Windows And Create A New Key Called WindowsUpdate

![4](https://user-images.githubusercontent.com/94680549/228785313-813ed459-998b-46f0-8fa4-a9f4f8179551.png)

![5](https://user-images.githubusercontent.com/94680549/228786052-a0e299cc-33cd-40f6-ac5b-124c600e0b8d.png)

4.Right Click On The Key WindowsUpdate And Create A New String Value Called TargetReleaseVersionInfo

![6](https://user-images.githubusercontent.com/94680549/228786723-c50c0eca-4c57-4d84-8a17-bcfc8a7ca9cc.png)

5.Right Click On The String Value TargetReleaseVersionInfo And Click On Modify And Set The String Value As Your Current Windows Version Or The Windows Version You Would Like To Update To 

![7](https://user-images.githubusercontent.com/94680549/228789209-e783a561-cc0b-4e55-b5e2-678d328f26e1.png)

![8](https://user-images.githubusercontent.com/94680549/228789251-0706c52c-450a-4c0f-93c9-a79ca580fa5f.png)

6. Right Click On The Key WindowsUpdate And Create A New DWORD(32-bit) Value Called TargetReleaseVersion

![9](https://user-images.githubusercontent.com/94680549/228790372-9c641881-4357-4876-865b-907d5fefd2bb.png)

7. Right Click On The DWORD Value TargetReleaseVersion And Set The DWORD Value To 1

![10](https://user-images.githubusercontent.com/94680549/228791418-9817decc-c4da-4556-9949-d535faba9870.png)

![11](https://user-images.githubusercontent.com/94680549/228792750-e5ed0972-0bde-4753-b08e-d1f295d749bc.png)

![12](https://user-images.githubusercontent.com/94680549/228793189-89403d74-485c-4e78-9295-1a839b00ec59.png)






