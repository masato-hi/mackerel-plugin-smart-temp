# mackerel-plugin-smart-temp
Add metrics of temperature obtained from S.M.A.R.T. to mackerel.

## Installation
#### Please install smartctl in advance.
for Ubuntu/Debian
```
sudo apt-get -y install smartmontools
```
for CentOS
```
sudo yum -y install smartmontools
```

#### Place mackerel-plugin-smart-temp and make it executable.
```
curl -o /usr/local/bin/mackerel-plugin-smart-temp https://raw.githubusercontent.com/masato-hi/mackerel-plugin-smart-temp/master/mackerel-plugin-smart-temp
chmod +x /usr/local/bin/mackerel-plugin-smart-temp
```

#### Please add the following contents to /etc/mackerel-agent/mackerel-agent.conf
```
[plugin.metrics.smart.temperature]
command = "mackerel-plugin-smart-temp"
```

#### Please restart mackerel-agent.
```
service mackerel-agent restart
```


## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/masato-hi/mackerel-plugin-smart-temp.


## License

The script is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

