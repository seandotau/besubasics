# Using a config file

Up until this point, we have used the command line to provide various parameters to Besu. Another way to provide these parameters is to use a configuration file or a config file. The advantage of a configuration file is that it can be saved and reused across different nodes at startups. To specify a config file we use the [--config-file](https://besu.hyperledger.org/en/stable/Reference/CLI/CLI-Syntax/#config-file) flag. 

```text
./besu --config-file=/home/username/Besu/configfile/myconfigfile_mainnet.toml
```

A third way to provide parameters to Besu is via environment variables. However, if the same parameter is provided in multiple locations, the order of precedence is as follows; Command line, environment variable, configuration file.

The configuration file is composed of a key/value pair. The key is the same name as the command line option mins the leading double dashes. Other specifications include; comma-separated lists on the command line are string arrays in the TOML file and file paths, hexadecimal numbers, URLs, and &lt;host:port&gt; values must be enclosed in quotes.

To move all our command line parameters into a configuration file create a file called myconfigfile.toml with the following.

```text
data-path="/home/username/Besu/database_mainnet"
network="mainnet"
rpc-http-enabled=true
```

{% hint style="info" %}
More often  that not, the configuration file will be in a special configuration folder so the command line will probably read 
{% endhint %}



