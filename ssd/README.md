# SSD

## Introduction

I have been using solid-state storage in various unix-like operating
systems since about 2002. Support for SSDs is much more complete in
Linux, these days, but there are still some gaps here and there.
Included in this subdirectory of the linux-utils repo are some of the
bridges for those gaps.

## Files

* udev/rules.d/60-ssd-scheduler.rules: Rule to set the "noop" I/O
  scheduler for any disk identified as non-rotational
* cron.weekly/fstrim: Runs fstrim on all mounted filesystems that
  support it
