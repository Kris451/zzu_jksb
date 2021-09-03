# 郑州大学健康上报
![img](https://img.shields.io/github/license/21wang12/zzu_jksb)

## 有什么特点？
该打卡程序超级轻量，简单到只有一个python文件，超级简易配置，只需填写账号密码即可运行。
程序程序可在后台无感运行。

## 环境
+ `python3`
+ 用于发送http请求的`requests`模块


## 用法：

1. 用记事本打开并修改`jksb.py`的第2行第3行，修改为自己的**账户名**和**密码**，修改完之后保存。
```python
# 将XXXX替换为学号和密码
id = "XXXXX"
pwd = "XXXXX"
```
2. 打开命令行，运行下列命令即可打卡。
```bash
python jksb.py
``` 
3. 如果提示未安装requests模块，请输入下面命令，并重新执行第2步
```bash
pip install requests
```

## 运行截图

图中对隐私信息进行了打码

![image](https://user-images.githubusercontent.com/38482259/125930325-8dbe6d10-27c9-4cfc-9b26-26ab1ca9d9e5.png)


## Q&A
+ 如何打开命令行？
  + 利用键盘的组合按键`win+r`，在弹出的窗口输入`cmd`并按下回车即可打开命令行

+ 如何查看自己是否安装了`python`?
  + 打开命令行，输入下面语句，如果返回了python的版本，说明已经安装
  ```bash
  python --version
  ```

+ 如何每日执行此程序？
  + 需要你有一台Linux服务器。服务器按照此教程：[crontab设置定时任务](https://segmentfault.com/a/1190000023186565#:~:text=%E5%9C%A8Linux%20%E4%B8%AD%EF%BC%8C%E5%8F%AF%E4%BB%A5%E4%BD%BF%E7%94%A8,%E5%86%99%E5%85%A5%E4%B8%80%E4%B8%AAcrontab%20%E6%96%87%E4%BB%B6%E3%80%82)进行配置
  + [GithubAction](https://www.ruanyifeng.com/blog/2019/09/getting-started-with-github-actions.html)也可以利用crontab设置定时任务，感谢 [@kris451](https://github.com/Kris451) 提供思路
  + 如果没有linux服务器，在windows上定时任务可以参考[windows定时执行python](https://www.jianshu.com/p/43676346b0be)
