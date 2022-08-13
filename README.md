# NITC Network Login

A script to manage logging into the NITC network, because logging into the captive portal and keeping that window alive isn't cool enough.

Just run this script, and keep the terminal window open in the background to manage the reauthentication timer. Close the window to logout of the network.

## To use the script

- Open the file and add your network login credentials as follows

```bash
expressions=("username:password" "user2:pass2")
# You're supposed to have only one login of course, but by the inexplicable alignment of the universe, if you somehow come into possession of some other credentials, you can add it here and everything in the list will be used randomly until successful authentication.
```

A desktop file is also included in the repo which you could move to `/usr/share/applications` or wherever your DE places desktop files.

Also, this is a Linux script, probably won't work on Windows. Can be translated to Powershell or whatever though.

## Options

| Option | Description                                 |
| ------ | ------------------------------------------- |
| -h     | Print the help menu                         |
| -o     | Run the script without the refresh timer    |
| -n     | Send notifications on network status update |
