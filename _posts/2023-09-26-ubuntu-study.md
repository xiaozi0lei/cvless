---
layout: post
title: ubuntu study
lead: ubuntu study

---

1. linux下使用命令`useradd -m test`创建新用户后，远程ssh登录后无法使用方向键，显示![方向键乱码](https://img-blog.csdnimg.cn/2021031418081582.png)

   因为在创建用户的时候，没有给用户明确指定使用的linux 的shell 类型，默认会使用 `/bin/sh` 不识别方向键，使用命令修改用户的默认 shell 类型为 bash 即可

   ```
   chsh
   根据提示符输入 /bin/bash
   ```

   

2. 1