#!/bin/bash

awk '{print $1}' logfile.txt | sort | uniq -c | sort -nr | head -8 | awk '{print $2, $1}'

