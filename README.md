# src-notices-actions
SRC每日公告爬取，并通过github actions自动运行
> lin9e@qq.com

# Usage
Github Actions自动运行python脚本实现，无需部署环境可在线运行，方便食用。

- 具体通知时间从`.github/workflows/src-notices-actions.yml`文件修改，如下为每日9点半运行一次脚本
```
on:
  schedule:
    - cron: '30 9 * * *'
  workflow_dispatch:
```
- 运行过程可通过src-notices-actions项目对应Actions处查看，调试
- 每日运行结果以txt文件形式存储于output目录

# 版本
### v0.1
- 基于Bywalks的OnTimeHacker, 在此基础上添加github actions自动运行脚本并提醒
- 暂时删除无法访问的src:guazi
- 更新字节SRC网站
