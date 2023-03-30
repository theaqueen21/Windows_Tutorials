# Disable Windows Updates Using The Registry

1.Open The Registry(regedit.exe)
>Press The Windows Key And R
```
Win+R
```
>Type
```
regedit.exe
```

![1](https://user-images.githubusercontent.com/94680549/228795710-4a6813be-2f10-4506-bf77-62c71473c126.png)

![2](https://user-images.githubusercontent.com/94680549/228795747-0c918fe0-ac12-4ef2-9d10-763ff3bfc2ce.png)

2. Navigate To

```
Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\
```

![3](https://user-images.githubusercontent.com/94680549/228797668-79bf334a-30c9-4b85-90a8-ff4e2159b5f1.png)

3. Right Click On The Windows Folder And Create A New Key Called WindowsUpdate

![4](https://user-images.githubusercontent.com/94680549/228797850-99ea94b2-5d59-45e0-83cd-c213b49a02e8.png)

![5](https://user-images.githubusercontent.com/94680549/228797886-b1c3135a-8201-4bf9-942c-97fcc822b7ce.png)

4. Right Click On The Key WindowsUpdate And Create A New String Value Called TargetReleaseVersionInfo

![6](https://user-images.githubusercontent.com/94680549/228798253-9737bd04-2489-45f7-9bd9-363532d3040e.png)

5. Right Click On The String Value TargetReleaseVersionInfo Click On Modify And Set The Value As Your Current Windows Version Or The Version You Would Like To Update To

![7](https://user-images.githubusercontent.com/94680549/228798846-28137ce4-d904-484d-982c-0fd98df0c1e1.png)

![8](https://user-images.githubusercontent.com/94680549/228798909-d747a227-8156-456b-87f4-75668c972b6e.png)

6. Right Click On The Key WindowsUpdate And Create A New DWORD(32-bit) Value Called TargetReleaseVersion

![9](https://user-images.githubusercontent.com/94680549/228799080-3887ac7f-5c11-4f0f-9076-f1ae405bf315.png)

7. Right Click On The DWORD(32-bit) Value And Modify Its Value To 1

![10](https://user-images.githubusercontent.com/94680549/228799271-9ef83a80-b54f-46f1-9462-19098b2b7db0.png)

![11](https://user-images.githubusercontent.com/94680549/228799291-9aaab0f1-5370-415d-ae52-7cd925e1a052.png)

![12](https://user-images.githubusercontent.com/94680549/228799336-80060a0c-38f4-45c5-883d-bb8c9c1d50ae.png)

Note: This Method Only Disables Windows Feature And Cumulative Updates And There Still Will Be Security Updates And Windows Defender Intelligence Updates
