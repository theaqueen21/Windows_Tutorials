# Disable Windows Updates Using Powershell

1.Open Powershell As Admin
>Press On The Start Button And Type Powershell And Run It As Admin

![1](https://user-images.githubusercontent.com/94680549/228802483-322e389e-33e3-4509-a483-d4482d9f056d.png)

![2](https://user-images.githubusercontent.com/94680549/228802507-dae4e956-ea79-4590-8cd1-bbcd8bd7ac3a.png)

2.Copy And Paste This Command

```
reg add HKLM\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate /f /v TargetReleaseVersion /t REG_DWORD /d 1
```

![3](https://user-images.githubusercontent.com/94680549/228803540-65d00284-4e51-46c5-a017-780a779ea491.png)

3.Copy And Paste This Command

```
reg add HKLM\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate /f /v TargetReleaseVersionInfo /t REG_SZ /d 1904
```
>Replace 1904 As Your Preference(With Either Your Current Windows Version Or The Version You Would Like To Update To)

![4](https://user-images.githubusercontent.com/94680549/228804088-49ab5c10-dad0-4d85-b97c-84084b5abf8e.png)

Note: This Method Only Disables Windows Feature And Cumulative Updates And There Still Will Be Security Updates And Windows Defender Intelligence Updates
