# Prometheus
`sudo adduser prometheus`

`wget https://github.com/prometheus/prometheus/releases/download/v2.32.1/prometheus-2.32.1.linux-amd64.tar.gz`

`tar -xvf prometheus-2.32.1.linux-amd64.tar.gz`

`sudo mkdir -p /data /etc/prometheus && cd prometheus-2.32.1.linux-amd64 && sudo mv prometheus promtool /usr/local/bin/`

`sudo mv consoles/ console_libraries/ /etc/prometheus/ && sudo mv prometheus.yml /etc/prometheus/prometheus.yml && sudo chown -R prometheus:prometheus /etc/prometheus/ /data/`

`cd && rm -rf prometheus*`

`sudo systemctl status prometheus`

![1](https://user-images.githubusercontent.com/61537053/175573330-85a4c324-4aaf-4476-b0ca-43149e925f24.png)

# Grafana
`sudo apt update`

`sudo apt-get install -y gnupg2 curl software-properties-common`

`curl https://packages.grafana.com/gpg.key | sudo apt-key add -`

`sudo add-apt-repository "deb https://packages.grafana.com/oss/deb stable main"`

`sudo apt update`

`sudo apt -y install grafana`

`sudo systemctl start grafana-server`

`sudo systemctl status grafana-server`

![2](https://user-images.githubusercontent.com/61537053/175573337-cd099086-7317-4368-87a1-aba4b6c7acd1.png)
