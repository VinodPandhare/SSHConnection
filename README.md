# In  this tutorial we earn How To Connect Ec2 Instance using windows powershell !!
# Fist Install Two Optional Features 👇
  # GoTo Setting >> Apps >> Optional Features >> Add an optional feautre >> Serach for >>  1. OpenSHH Client & Install.  2. OpenSHH Sever & Install.
 # After that goto the Pem file location then right click & Open in Tereminal & Pest this commands 👇 
# Commands for change file permmisson 
```
$path = ".\Replacewithyourfilename.pem"

icacls.exe $path /reset
icacls.exe $path /GRANT:R "$($env:USERNAME):(R)"
icacls.exe $path /inheritance:r
```

# Then Press Enter Two Times 
