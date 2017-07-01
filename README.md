# HTTP Server
## Prerequisites
- Terminal (UNIX, GNU/LINUX)
- Command Prompt/[PowerShell](https://msdn.microsoft.com/en-us/powershell/mt173057.aspx) (Windows)
- [PHP 7](http://php.net/downloads.php) or greater
- Add PHP to your environment variable `PATH` to make it available via `php` in your Terminal/Command Prompt/PowerShell
- [Git](https://git-scm.com/download/) (CLI or GUI) (optional)
## Download
### With Git
```shell
$ git clone https://github.com/aminnairi/httpserver
```
![git_clone](https://j.gifs.com/P1Brw4.gif)
### Without Git
![without_git_clone](https://j.gifs.com/lOqDlM.gif)
## How to use the script
Move the script to the root of your web server's folder and execute the following commands.
All commands explained later are cumulable (except for the help command).
### Simple server
```shell
$ php httpserver
```
![php_httpserver](https://j.gifs.com/RgEwGO.gif)
### Custom document root
```shell
$ php httpserver --base ./docs/
$ # or
$ php httpserver -b ./docs/
```
![http_server_base](https://j.gifs.com/mwrG49.gif)
Where `./docs/` is the path to the document root of your choice. Default is `./`.
### Custom port
```shell
$ php httpserver --port 8080
$ # or
$ php httpserver -p 8080
```
![php_httpserver_port](https://j.gifs.com/P1Bry1.gif)
Where `8080` is the desired port from which the server can be reached. Default is `8888`.
### Opened to the outside world
```shell
$ php httpserver --open
$ # or
$ php httpserver -o
```
![php_httpserver_open](https://j.gifs.com/GZpg08.gif)
Tells the script to open the web server to be available outside the loopback network. It basically sets the host parameter to `0.0.0.0`. Default is `localhost`.
### Get the help manual
```shell
$ php httpserver --help
$ # or
$ php httpserver -h
```
![php_httpserver_help](https://j.gifs.com/2RLOMN.gif)
Display the manual as in a man page with all the above commands described. Using this option will prevent the built-in web server to start.
## Grab the latest version after cloning with Git
```shell
$ git pull
```
