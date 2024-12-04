> [!CAUTION]
> The repository is in progress, please wait until the creator finish it.

# PumukyDev Web Server

This is my **self hosted web server**. At the moment it is hosted in my laptop with arch linux so **do not expect great availability** (In a few months it will be running 24/7 in a Raspberry Pi)

## Download

## Configuration

## Features
* Has a simple, but intuitive and usable User Interface.
* URL shortener tool.
* Status page.
* logo.png for some tests.
* Automatic provisioning made with Vagrant.
* /admin and /status password protection.
* Dynamic DNS configuration to autoconfigure my new home ip if it changes.

## URL Shortener in action...

![showing url-shortener](assets/screencasts/url-shortener.gif)

## Other

<details>
    <summary>
        <b>Files structure</b></summary><br/>

This is the my proyect files structure:

```
.
├── apache_exporter.service
├── compose.yml
├── config
│   ├── apache2
│   │   ├── apache2.conf
│   │   ├── certs
│   │   │   ├── intermediate
│   │   │   │   ├── intermediate1.cer
│   │   │   │   └── intermediate2.cer
│   │   │   ├── _.pumukydev.com_private_key.key
│   │   │   └── pumukydev.com_ssl_certificate.cer
│   │   └── sites-available
│   │       └── pumukydev.conf
│   ├── dynamic-dns
│   │   ├── dyndns-cronjob
│   │   ├── get_url
│   │   │   └── dyndns.sh
│   │   └── README.md
│   └── monitoring
│       ├── grafana
│       │   ├── dashboard.json
│       │   ├── dashboard.yml
│       │   ├── datasources.yml
│       │   └── grafana.ini
│       ├── images
│       │   ├── grafana_change_passwd.jpg
│       │   ├── grafana_connections.jpg
│       │   ├── grafana_graph.jpg
│       │   ├── grafana_login.jpg
│       │   ├── grafana_prometheus.jpg
│       │   ├── prometheus_add_source.jpg
│       │   ├── prometheus_settings.jpg
│       │   └── prometheus_succed.jpg
│       ├── prometheus
│       │   └── prometheus.yml
│       └── README.md
├── htdocs
│   ├── admin
│   │   └── index.php
│   ├── errors
│   │   ├── error404.php
│   │   └── README.md
│   ├── images
│   │   └── favicon.png
│   ├── includes
│   │   ├── footer.php
│   │   └── header.php
│   ├── index.php
│   ├── logo.png
│   ├── shortener
│   │   ├── get_long_url.sh
│   │   ├── get_txt.sh
│   │   ├── get_zoneId.sh
│   │   ├── index.php
│   │   ├── post_txt.sh
│   │   ├── redirect.php
│   │   └── urlshortener.php
│   ├── status
│   │   └── index.php
│   ├── style
│   │   └── style.css
│   └── tools
│       └── index.php
├── playbooks
│   ├── main.yml
│   ├── tasks
│   │   ├── apache.yml
│   │   ├── dyndns.yml
│   │   └── monitoring.yml
│   └── vars
├── README.md
└── Vagrantfile
```
</details>

## License

## Contribute

Want to contribute? There are multiple ways you can contribute to this project. Here are some ideas:

* 📃 [Translate the web into multiple languages!](./CONTRIBUTING.md#translations)
* 🐛 [Fix some easy issues](CONTRIBUTING.md#coding)
* 💡 [Or check out some other issues](CONTRIBUTING.md#need-ideas) (or translate them).