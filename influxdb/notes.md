# InfluxDB

## Install InfluxDB

portal.influxdata.com/downloads

```
wget https://dl.influxdata.com/influxdb/releases/influxdb2-2.7.6_linux_amd64.tar.gz
tar xvfz influxdb2-2.7.6_linux_amd64.tar.gz
```

RHEL
```
# influxdata-archive_compat.key GPG fingerprint:
#     9D53 9D90 D332 8DC7 D6C8 D3B9 D8FF 8E1F 7DF8 B07E
cat <<EOF | sudo tee /etc/yum.repos.d/influxdata.repo
[influxdata]
name = InfluxData Repository - Stable
baseurl = https://repos.influxdata.com/stable/\$basearch/main
enabled = 1
gpgcheck = 1
gpgkey = https://repos.influxdata.com/influxdata-archive_compat.key
EOF

sudo yum install influxdb2
```

## Install Telegraf open source data collector

```
wget https://dl.influxdata.com/telegraf/releases/telegraf-1.31.0_linux_amd64.tar.gz
tar xf telegraf-1.31.0_linux_amd64.tar.gz
```

RHEL
```
# influxdata-archive_compat.key GPG fingerprint:
#     9D53 9D90 D332 8DC7 D6C8 D3B9 D8FF 8E1F 7DF8 B07E
cat <<EOF | sudo tee /etc/yum.repos.d/influxdata.repo
[influxdata]
name = InfluxData Repository - Stable
baseurl = https://repos.influxdata.com/stable/\$basearch/main
enabled = 1
gpgcheck = 1
gpgkey = https://repos.influxdata.com/influxdata-archive_compat.key
EOF

sudo yum install telegraf
```


