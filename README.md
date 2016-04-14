gw-buaa
==========
Login to gw.buaa.edu.cn

You should have a gw-buaa.conf in /etc/

```
USERNAME:Your Username
PASSWORD:Your Password(raw)
```
FOR `systemd`
```sh
	sudo cp gw-buaa@.service /usr/lib/systemd/system/gw-buaa@.service
	sudo systemctl start gw-buaa@[Your INTERFACE Name].service
```
FOR `SysVinit`
```sh
	sudo cp rc.d/gw-buaa /etc/rc.d/gw-buaa
	sudo update-rc.d gw-buaa default
```
