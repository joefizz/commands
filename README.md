# commands
commands i hvae to keep searching for

## Change .pem file permissions in Windows

### Current user
```
icacls.exe your_key_name.pem /reset
icacls.exe your_key_name.pem /grant:r ""%username%:(R)
icacls.exe your_key_name.pem /inheritance:r
```

### AzureAD user:

```
icacls.exe your_key_name.pem /reset
icacls.exe your_key_name.pem /grant:r "AzureAD\username:(R)"
icacls.exe your_key_name.pem /inheritance:r
```
