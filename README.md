# auto_sign-python3
自动签到程序，Python3， 目前支持字幕组（人人影视）, 炫音音乐论坛

运行zimuzu.py前请先确认可以用IE浏览器正常打开http://www.zimuzu.tv  主程序里your_username 和 your_password改成自己的用户名和密码,自动签到是为了提高等级，获取更多美剧、电影资源的下载权限

  crontab 定时执行zimuzu.py：：
  在Python文件头部加入（已加入）
  #!/usr/bin/env/python
  更改zimuzu.py的权限，使其可以执行:chmod a+x zimuzu.py
  用当前用户执行，可以用命令crontab -e 来打开一个vi编辑自己的任务
  crontab -e 
  30 12 * * * python3 /root/python/zimuzu.py #每天12.30执行一次。


炫音音乐论坛http://bbs.musicool.cn/，因为登录要填验证码（较复杂），采用cookie登录， 所以需要把文件里的cookie改为自己在chrome登录后的cookie， 自动登录和自动回复都是为了获取音符来下载音乐，详见（http://bbs.musicool.cn/thread-598441-1-1.html）
