# Apache Solr <=8.2.0 Velocity Template 0day Exploit

Exploit: https://github.com/k8gege/SolrExp<br>
Cscan: https://github.com/k8gege/K8CScan<br>
### 环境
下载Solr 8.2.0添加core,默认配置即可。7.x版本自带core
### 配置
0x001 批量URL配置Cscan.ini<br>
[Cscan]<br>
exe=F:\Python279\python.exe<br>
arg=exp.py $ip$ whoami<br>
0x002 批量C段配置Cscan.ini<br>
[Cscan]<br>
exe=F:\Python279\python.exe<br>
arg=exp.py http://$ip$:8983 whoami<br>
### 利用
单个: python exp.py url cmd<br> 或 Cscan url<br>
批量C段: Cscan 192.168.1.8/24<br>
批量URL: Cscan (同目录放url.txt)

<img src=https://github.com/k8gege/SolrExp/blob/master/Solr0day.gif>
