# Knife docker wrapper

Possible use like this:

```bash
knifed() {
  docker run --rm -ti --volume=/etc/chef:/etc/chef --volume=`pwd`/.chef:/.chef knife knife "$@" -c /.chef/knife.rb
}
```
