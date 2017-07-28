# asterisk2ch2o

该脚本用于迁移5.x asterisk中的数据至ch2o


### 步骤
1. 登录目的主机
2. 安装mysql，并配置用户密码
3. 执行该脚本

### 说明

```
USAGE: ./asterisk2ch2o [-h] src_host src_user src_password dst_user dst_password

DESCRIPTION:
    This script uses to transfer data from asterisk to ch2o. You need login to destination host and execute this script.
    If you can't see congratulations, that means failed. you can check asterisk2ch2o.log for details.

    src_host        source host where data locate. can be ip or domain.
    src_user        the user of source database.
    src_password    the password of source database. must be '' if without password.
    dst_user        the user of destination database.
    dst_password    the password of destination database. must be '' if without password.

OPTIONS:
    -h                Show this help message and exit

EXAMPLES:
    ./asterisk2ch2o localhost root 123456 root 123456
    ./asterisk2ch2o localhost root 123456 root ''
```

### 示例

```
asterisk2ch2o localhost root 123456 root 123456
```
