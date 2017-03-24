# Knife docker wrapper

Possible use like this:

```bash
knifed() {
  docker run --rm -ti --volume=/etc/chef:/etc/chef --volume=`pwd`/.chef:/.chef milanaleksic/knifed knife "$@" -c /.chef/knife.rb
}
```
