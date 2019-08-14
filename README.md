This is a basic [asdf-vm](https://github.com/asdf-vm/asdf) plugin for [Apache
Kafka](https://kafka.apache.org/). It's based off of (read: mostly copy-pasta
of) the
[asdf-elasticsearch](https://github.com/mikestephens/asdf-elasticsearch) plugin
currently.

## Install
```
asdf plugin-add elasticsearch https://github.com/mikestephens/asdf-elasticsearch.git
```

See the [asdf](https://github.com/asdf-vm/asdf) readme for instructions on how to install & manage versions of kafka.

```
asdf install kafka 2.3.0
asdf local kafka 2.3.0
```

### Running Kafka

```
zookeeper-server-start.sh $(asdf where kafka)/config/zookeeper.properties
```

```
kafka-server-start.sh $(asdf where kafka)/config/server.properties
```

## TODO
 - [ ] Cleanup the code a bit in install to make the intents clearer, and document it a bit
 - [ ] More versions?
 - [ ] Travis build/testing and [official plugin addition](https://github.com/asdf-vm/asdf-plugins)?
