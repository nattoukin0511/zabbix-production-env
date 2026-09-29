#概要
Zabbixの構築を通して、本番環境の構築手順やトラブルシューティングのプロセスを成果物としてまとめる。

---
#1.構築手順
　sudo apt update

　# Zabbix Server導入
　sudo apt install zabbix-server-pgsql
　sudo apt install zabbix-agent

　# サービス起動
　sudo systemctl start zabbix-server
　sudo systemctl start zabbix-agent

　# 自動起動設定
　sudo systemctl enable zabbix-server
　sudo systemctl enable zabbix-agent
---

#2発生したエラー
　1. Agentが緑にならない
　 症状Hostが監視対象として正常表示されない

　2. 通信エラー
   症状Zabbix ServerからAgentへ接続できない

---

#3原因調査
 1　systemctl status zabbix-agent
　　cat /etc/zabbix/zabbix_agentd.conf
　　journalctl -u zabbix-agent

 2　ss -tulpn | grep 10050
　  telnet <IP> 10050
 ---
#4解決方法
 #1.HOST IP HOSTNAME記載
/etc/zabbix/zabbix_agentd.conf
 Server=
 ServerActive=
 Hostname=
修正後
 sudo systemctl restart zabbix-agent

 2．/etc/zabbix/zabbix_agentd.conf
  Server IP設定を修正後
  sudo systemctl restart zabbix-agent

---
#5.修正ファイル
　/etc/zabbix/zabbix_agentd.conf
---
#6.学んだこと
 ZabbixではHostnameがGUIのHost名と一致している必要がある。
 Agent設定ファイル修正後は再起動が必要
 Agentの疎通にはIP設定とポート10050が重要。
 通信障害時はサービス状態とLISTENポートを確認する。

----
付録
　apt update
　apt install zabbix-server-pgsql
　apt install zabbix-agent
　systemctl start zabbix-server
　systemctl start zabbix-agent
　systemctl enable zabbix-server
　systemctl enable zabbix-agent
　systemctl restart zabbix-agent
　systemctl status zabbix-agent