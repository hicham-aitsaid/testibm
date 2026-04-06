dsmadmc -id=admin -pa=P@ssw0rdP@ssw0rd query schedule WIN_DOM -dataonly=yes -comma | for /f "tokens=2 delims=," %a in ('findstr /v "^$"') do @echo %a
