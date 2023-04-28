# Check Your HDD's Status Using CMD

>Check If Your HDD Is Failing

# Steps: 

1.Press The Windows Key, Search CMD And Run It As Administrator

![1](https://user-images.githubusercontent.com/94680549/235113749-5f6efd22-048d-4a55-8b29-c3a0be70da83.jpg)

![2](https://user-images.githubusercontent.com/94680549/235113780-d2e46c4d-a735-4ade-b5c1-521b626920bb.jpg)

2.Run The Command

```
wmic diskdrive get status,model
```
>If Status Reads "Bad", "Unknown", Or "Caution" Hardware Failure Could Be Soon

![55](https://user-images.githubusercontent.com/94680549/235116216-e396ceb8-885a-4028-88b5-41f99e3f0a70.jpg)

>Determining Drive Predictive Failure

3.Run The Command

```
wmic /namespace:\\root\wmi path MSStorageDriver_FailurePredictStatus
```
>If PredicFailure Reads False, Then Drive Is Working Properly And Not Going To Have Any Issues

![66](https://user-images.githubusercontent.com/94680549/235117765-907d6b55-58a6-4d63-83bb-72085916c264.jpg)

