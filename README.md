# Learn Elasticsearch

> ## Install in Mac OS with Homebrew

1. To install with Homebrew, you first need to tap the Elastic Homebrew repository:

```bash
brew tap elastic/tap
```

2. Use brew install to install the default distribution of Elasticsearc:

```
brew install elastic/tap/elasticsearch-full
```

> ## Directory layout for Homebrew installs

When you install Elasticsearch with brew install the config files, logs, and data directory are stored in the following locations.

|Type|Description|Default Location|Setting|
|----|-----------|----------------|-------|
|home|Elasticsearch home directory or `$ES_HOME`|`/usr/local/var/homebrew/linked/elasticsearch-full`||
|bin|Binary scripts including elasticsearch to start a node and elasticsearch-plugin to install plugins|`/usr/local/var/homebrew/linked/elasticsearch-full/bin`||
|conf|Configuration files including `elasticsearch.yml`|`/usr/local/etc/elasticsearch`|`ES_PATH_CONF`|
|data|The location of the data files of each index / shard allocated on the node. Can hold multiple locations.|`/usr/local/var/lib/elasticsearch`|`path.data`|
|logs|Log files location.|`/usr/local/var/log/elasticsearch`|`path.logs`|
|plugins|Plugin files location. Each plugin will be contained in a subdirectory.|`/usr/local/var/homebrew/linked/elasticsearch/plugins`||
