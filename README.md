99Gotty
Run docker container in web browser 

```bash
Steps to install gotty
curl -o /etc/yum.repos.d/home_radiorabe_misc.repo http://download.opensuse.org/repositories/home:/radiorabe:/misc/CentOS_7/home:radiorabe:misc.repo
yum install gotty-bin

/opt/gotty/bin/gotty [CMD]


/opt/gotty/bin/gotty -w -p "9000" -c "username:password" docker run -it <dokcer image name>

/opt/gotty/bin/gotty
NAME:
   gotty - Share your terminal as a web application

USAGE:
   gotty [options] <command> [<arguments...>]

VERSION:
   1.0.1

OPTIONS:
   --address value, -a value     IP address to listen [$GOTTY_ADDRESS]
   --port value, -p value        Port number to listen (default: "8080") [$GOTTY_PORT]
   --permit-write, -w            Permit clients to write to the TTY (BE CAREFUL) [$GOTTY_PERMIT_WRITE]
   --credential value, -c value  Credential for Basic Authentication (ex: user:pass, default disabled) [$GOTTY_CREDENTIAL]
   --random-url, -r              Add a random string to the URL [$GOTTY_RANDOM_URL]
   --random-url-length value     Random URL length (default: 8) [$GOTTY_RANDOM_URL_LENGTH]
   --tls, -t                     Enable TLS/SSL [$GOTTY_TLS]
   --tls-crt value               TLS/SSL certificate file path (default: "~/.gotty.crt") [$GOTTY_TLS_CRT]
   --tls-key value               TLS/SSL key file path (default: "~/.gotty.key") [$GOTTY_TLS_KEY]
   --tls-ca-crt value            TLS/SSL CA certificate file for client certifications (default: "~/.gotty.ca.crt") [$GOTTY_TLS_CA_CRT]
   --index value                 Custom index.html file [$GOTTY_INDEX]
   --title-format value          Title format of browser window (default: "GoTTY - {{ .Command }} ({{ .Hostname }})") [$GOTTY_TITLE_FORMAT]
   --reconnect                   Enable reconnection [$GOTTY_RECONNECT]
   --reconnect-time value        Time to reconnect (default: 10) [$GOTTY_RECONNECT_TIME]
   --timeout value               Timeout seconds for waiting a client (0 to disable) (default: 0) [$GOTTY_TIMEOUT]
   --max-connection value        Maximum connection to gotty, 0(default) means no limit (default: 0) [$GOTTY_MAX_CONNECTION]
   --once                        Accept only one client and exit on disconnection [$GOTTY_ONCE]
   --permit-arguments            Permit clients to send command line arguments in URL (e.g. http://example.com:8080/?arg=AAA&arg=BBB) [$GOTTY_PERMIT_ARGUMENTS]
   --close-signal value          Signal sent to the command process when gotty close it (default: SIGHUP) (default: 1) [$GOTTY_CLOSE_SIGNAL]
   --width value                 Static width of the screen, 0(default) means dynamically resize (default: 0) [$GOTTY_WIDTH]
   --height value                Static height of the screen, 0(default) means dynamically resize (default: 0) [$GOTTY_HEIGHT]
   --config value                Config file path (default: "~/.gotty") [$GOTTY_CONFIG]
   --version, -v                 print the version


```
