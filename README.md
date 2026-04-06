@echo off
title IBM Spectrum Protect - Register Node Script

:: Prompt user for inputs
set /p NODE_NAME=Enter node name: 
set /p DOMAIN_NAME=Enter domain name: 
set /p NODE_PASSWORD=Enter node password: 

:: Optional: Admin credentials (edit if needed)
set ADMIN_USER=admin
set ADMIN_PASS=password

echo.
echo Registering node...
echo.

:: Run the register node command
dsmadmc -id=%ADMIN_USER% -password=%ADMIN_PASS% ^
"register node %NODE_NAME% %NODE_PASSWORD% domain=%DOMAIN_NAME%"

echo.
echo Node registration command executed.
pause