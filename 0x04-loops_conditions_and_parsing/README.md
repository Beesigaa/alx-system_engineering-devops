#!/usr/bin/env bash
# Apache 2

awk '{ print $1, $9 }' apache-access.log | sort | uniq -c | sort -k1 -r
