# In  this tutorial we learn How To Connect Ec2 Instance using Windows Powershell!!
# First Install Two Optional Features 👇
  # GoTo Setting >> Apps >> Optional Features >> Add an optional feautre >> Serach for >>  1. OpenSSH Client & Install.  2. OpenSHH Sever & Install.
 # After that go to the Pem file location then right-click & Open in Terminal & Pest these commands 👇 
# Commands for change file permission 
```
# Set the path to the security key & Replace it with your KeyPair Name 
$path = "C:\Users\HP\Downloads\Security_key.pem"

# Reset the permissions of the file
icacls.exe $path /reset

# Grant read permissions to the current user
$username = $env:USERNAME
icacls.exe $path /GRANT:R "${username}:(R)"

Write-Host "Permissions set successfully for $path"

```

# Then Press Enter Two Times 
