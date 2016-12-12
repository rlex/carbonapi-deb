# carbonapi-deb
Debian/ubuntu packaging for https://github.com/dgryski/carbonapi

### Short howto:
1. clone repo
2. apt-get install devscripts dh-golang golang-go git
3. cd to carbonapi-deb directory
4. run dpkg-buildpackage -sa
5. look for .deb in carbonapi-deb/../

### Notes:
1. There is only systemd service file, no classical init (i'm too lazy), so this might not work on older debian/ubuntu
2. There is no real config for carbonapi since it uses arguments for configuration, so look into /etc/default/carbonapi 
3. Since carbonapi is unversioned you will always build latest master from https://github.com/dgryski/carbonapi
