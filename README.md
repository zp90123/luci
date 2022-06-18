# OpenWrt luci feed

## Description

1. https://github.com/coolsnowwolf/luci.git
2. https://github.com/kenzok8/openwrt-packages.git
3. https://github.com/fw876/helloworld.git

## Usage

This feed is enabled by default. Your feeds.conf.default (or feeds.conf) should contain a line like:
```
src-git small https://github.com/kenzok8/small.git
src-git luci https://github.com/openwrt/luci.git
```

To install all its package definitions, run:
```
./scripts/feeds update luci
./scripts/feeds install -a -p luci
```

