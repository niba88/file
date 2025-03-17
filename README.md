# Linux一键下载与启动

```bash
screen -ls | grep newbot && screen -X -S newbot quit; sleep 2; wget -O grid_strategy https://github.com/niba88/file/releases/download/bug/grid_strategy && chmod +x grid_strategy && screen -dmS newbot ./grid_strategy
```

## 命令说明

1. `screen -ls | grep newbot && screen -X -S newbot quit`
   - 检查是否存在名为"newbot"的screen会话，如果存在则终止它

2. `sleep 2`
   - 等待2秒，确保之前的screen会话完全关闭

3. `wget -O grid_strategy https://github.com/niba88/file/releases/download/bug/grid_strategy`
   - 从GitHub下载最新版本的grid_strategy程序

4. `chmod +x grid_strategy`
   - 给下载的文件添加执行权限

5. `screen -dmS newbot ./grid_strategy`
   - 在新的screen会话中启动程序，会话名为"newbot"
