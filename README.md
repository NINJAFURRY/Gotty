99Gotty
Run docker container in web browser 

```bash
Steps to install gotty
curl -o /etc/yum.repos.d/home_radiorabe_misc.repo http://download.opensuse.org/repositories/home:/radiorabe:/misc/CentOS_7/home:radiorabe:misc.repo
yum install gotty-bin

/opt/gotty/bin/gotty [CMD]


/opt/gotty/bin/gotty -w -p "9000" -c "username:password" docker run -it <dokcer image name>
```
