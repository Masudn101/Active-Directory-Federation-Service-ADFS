# Active-Directory-Federation-Service-ADFS
Windows Server ADFS commands


### Install ADFS

```
Install-WindowsFeature adfs-federation -IncludeManagementTools
```

```

# Define the federation service name and the SSL certificate thumbprint
$federationServiceName = "fs.yourdomain.com"
$certThumbprint = "YOUR_CERTIFICATE_THUMBPRINT"

# Create the ADFS farm
Install-AdfsFarm -CertificateThumbprint $certThumbprint -FederationServiceDisplayName "Your Federation Service" -FederationServiceName $federationServiceName -Credential (Get-Credential)

```


```
Add-KdsRootKey -EffectiveImmediately
```
![Screenshot_1](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/78078ec3-e96a-4449-9fbe-0b012c3edb78)

![Screenshot_2](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/fec38e5b-da7b-4c2a-8677-99b7b816c2c1)

![Screenshot_3](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/2c033ae3-b3fe-4a34-91ba-0a924705fd93)

![Screenshot_4](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/0b43cb1d-f8d8-410f-a8ba-5f2718b62ab8)

![Screenshot_5](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/1ad0bc4c-ad5c-46c9-a886-4d977382b838)

![Screenshot_6](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/4d82317e-bcd5-49e5-b102-51c0be08789c)
![Screenshot_7](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/5fb7e886-3006-4176-9c64-32cbb20a2b3b)

![Screenshot_8](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/36098455-2a98-4c09-a430-af2cdaa526d6)

![Screenshot_9](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/febe1cad-1e3a-48a8-b7fd-7f5039e3411a)

![Screenshot_11](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/4d040eea-0c3a-4f46-b961-d97c9263032d)
![Screenshot_12](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/f7fdf309-6d8f-446e-bd12-c73e1fc50331)

![Screenshot_13](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/64e96ae1-f0fa-400d-b20b-5f8372fd9de8)
![Screenshot_14](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/8e50ca97-4751-4379-b927-d6d05c913e50)



![Screenshot_15](https://github.com/0xMasud101/Active-Directory-Federation-Service-ADFS/assets/39289859/00254020-2c26-4f74-b014-f3c7daa23570)




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


