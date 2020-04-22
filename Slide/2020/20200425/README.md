### edit 2020/4/22

使用 容器 來執行 smokeping
使用 -v 選項 掛載 自訂的 Alert / Database / General / Presentation / ssmtp.conf / Targets


Azure 環境
### # docker run --rm -d -e TZ=Asia/Taipei -v /root/Alerts:/config/Alerts  -v /root/Database:/config/Database -v /root/General:/config/General  -v /root/Presentation:/config/Presentation -v /root/ssmtp.conf:/config/ssmtp.conf  -v /root/Targets:/config/Targets -p 80:80 linuxserver/smokeping


