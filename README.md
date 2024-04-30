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


To Check

```
(Get-AdfsProperties).enableidpinitiatedsignonpage
```

```
Set-AdfsProperties -EnableIdPInitiatedSignonPage $true
```

```
(Get-AdfsProperties).enableidpinitiatedsignonpage
```


