# Active-Directory-Federation-Service-ADFS
Windows Server ADFS commands


### Install ADFS

```
Install-WindowsFeature adfs-federration -IncludeManagementTools
```

```
Add-KdsRootKey -EffectiveImmediately
```



![Screenshot 2024-04-30 at 10 15 05 PM](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/ff878e3a-37e4-41fb-8dc4-2d8e7de06b31)



To Check windows server 2012 it has by default.... no need these commands...
![Screenshot 2024-05-01 at 11 48 04 AM](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/f87ebaac-9510-47ce-bd5a-d81e3bd566a1)

https://adfs.macro.com/adfs/ls/IdPInitiatedSignon

```
(Get-AdfsProperties).enableidpinitiatedsignonpage
```

```
Set-AdfsProperties -EnableidPinitiatedSignonPage $true
```

```
(Get-AdfsProperties).enableidpinitiatedsignonpage
```


