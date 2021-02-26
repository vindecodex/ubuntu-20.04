# Installing tar.gz files

1. extract downloaded tar.gz file.

2. rename the file according to its name.

3. move the folder to /opt/ - this is where original application will be put.

  `sudo mv ~/Download/[app_name] /opt/`

4. create symbolic link

  `sudo ln -s /opt/[app_name]/[executable_file] /usr/bin/[app_name]

5. creating desktop icon

  `sudo vi /usr/share/applications/app_name.desktop`

  paste this and configure according your situation.

```bash
[Desktop Entry]
Encoding=UTF-8
Name=[app_name]
Exec=[app_name]
Icon=/opt/[app_name]/app/resources/app/assets/icon.png
Terminal=false
Type=Application
Categories=Development
```

Now Your Application is searchable and can be run through command: app_name
