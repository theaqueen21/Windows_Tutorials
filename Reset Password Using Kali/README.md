# Can't Login To Windows ? Reset The Password In Few Minutes
> Note: You Will Require A USB Drive And A Second Device For This Method

# 1 Download Kali Linux And Create A Bootable USB Drive

0. Download

> Download Kali: https://cdimage.kali.org/kali-2023.1/kali-linux-2023.1-live-amd64.iso

> Download Kali(From Mirror): https://mirrors.ocf.berkeley.edu/kali-images/kali-2023.1/kali-linux-2023.1-live-amd64.iso

> Download Balena Etcher: https://github.com/balena-io/etcher/releases/download/v1.18.4/balenaEtcher-Portable-1.18.4.exe

1. Run Balena Etcher As Administrator

![1](https://user-images.githubusercontent.com/94680549/235920772-e6e28bf1-05cb-48ee-9e3d-84860e5da57e.jpg)

2. Select The ISO You Just Downloaded

![2](https://user-images.githubusercontent.com/94680549/235920910-411a51b9-7eff-4778-a956-7e85ca237113.jpg)

![3](https://user-images.githubusercontent.com/94680549/235920927-5631ebd4-1a88-44d2-8dd0-4447d9755753.jpg)

3. Flash The USB

![4](https://user-images.githubusercontent.com/94680549/235920987-3680683e-d99a-4826-ac64-2ca492ce1a75.jpg)

![5](https://user-images.githubusercontent.com/94680549/235921036-1b773b16-0116-4f72-926e-3c8cd76cf630.jpg)

# 2 Boot Into Kali And Unlock The Account

0. Boot Into Kali Live And Select Kali Forensics As It Has The Tool We Need For The Account Unlock

![7](https://user-images.githubusercontent.com/94680549/235921293-f8f09ed0-5432-4327-8d67-70e9093d1629.jpg)

1. Open The Drive Containing Windows And Go To Windows/System32/config

![8](https://user-images.githubusercontent.com/94680549/235921728-4bb08393-f32d-4585-8f0c-a6826de1f035.jpg)

![9](https://user-images.githubusercontent.com/94680549/235922037-da00c4a3-1bc8-4136-aae7-2a95813238e1.jpg)

![10](https://user-images.githubusercontent.com/94680549/235921981-f8779044-1d0b-40b0-b76b-39a9a7576f98.jpg)

![11](https://user-images.githubusercontent.com/94680549/235922061-2f32b176-9494-4032-a57b-64ea9fb414c1.jpg)

2. Open The Terminal In The Directory

![12](https://user-images.githubusercontent.com/94680549/235922177-9364d57d-080a-4d6d-a416-ce354132f854.jpg)

3. Run The Command Below To List All The Users In The SAM File

```
chntpw -l SAM
```
![13](https://user-images.githubusercontent.com/94680549/235923135-994e2fae-2df5-405a-8a27-f512720489b6.jpg)

![144](https://user-images.githubusercontent.com/94680549/235923118-6e13e2fd-1292-44b7-8e28-9686dcc1562c.jpg)

4. Run The Commands Below To Reset The Preferred User Account

```
chntpw -u [User] SAM
```

![14](https://user-images.githubusercontent.com/94680549/235923391-fe807894-e066-43f0-8a2d-4ad6b71078b0.jpg)

![15](https://user-images.githubusercontent.com/94680549/235923607-be68371e-ecc0-4003-9989-3367bc443400.jpg)

![16](https://user-images.githubusercontent.com/94680549/235923694-0171f892-68a3-4120-a0da-356128e356fb.jpg)

![17](https://user-images.githubusercontent.com/94680549/235923729-7eb111be-f5c5-4318-b557-e3ce2e37cc13.jpg)

![18](https://user-images.githubusercontent.com/94680549/235923752-148355ee-5425-42c3-9ce7-9ee1d84280cd.jpg)

5. Once You Are Done Restart Back To Windows 

![19](https://user-images.githubusercontent.com/94680549/235923924-3629392e-69df-4afb-93b5-7bbc8b30c732.jpg)

6. Once Windows Boots It Will Automatically Log Into The Unlocked Account

![20](https://user-images.githubusercontent.com/94680549/235924067-bb817193-d70b-4a81-b3a8-061aef166075.jpg)
