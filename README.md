# Auto Punch-In Pica
自动"打哔咔"(签到).

(APP -> 个人中心 -> 右上角编辑按钮下面的图标 -> 打哔咔)

# Why
打哔咔可以提升用户经验, 建议使用 `cron` 每日定时打哔咔.

签到一次加 10 点经验, 但是升到二级(发送评论所需的最低等级)却需要 200 经验, 这简直是强人所难, 营养完全跟不上.

# How
本程序需要用户名和密码来实现登陆.

用户名和密码可以写在配置文件中或由命令行参数传入.

项目目录下的 `_config.ini` 是配置文件示例, 创建一份副本并命名为 `config.ini`, 如果你没有看到这份文件, 请使用以下示例作为文件内容

```ini
[DEFAULT]
email = yourEmail
password = yourPassword
```

若需要通过命令行参数来传入登陆信息, 见下方示例

```bash
python main.py yourEmail yourPassword
```

命令行参数的优先级高于配置文件.

若有任何问题请提交 issue.

# License
Apache 2.0
