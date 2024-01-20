# A Kernel Seedling
TODO: intro
Create a module we can load into the kernel to report how many
processes are running.

## Building
```shell
TODO: cmd for build
make
sudo insmod proc_count.ko
cat /proc/count
```

## Running
```shell
TODO: cmd for running binary
cat /proc/count
python -m unittest

```
TODO: results?
I ran a few separate times and got numbers between 160 and 163.
The results seem to be consistent, barring a few points when it
seemed like my VirtualBox was bugging.


## Cleaning Up
```shell
TODO: cmd for cleaning the built binary
sudo rmmod proc_count.ko
rm -r __pycache__
```

## Testing
```python
python -m unittest
```
TODO: results?
I failed FFF a few times because I had inserted the module before testing.
After removing the module and making clean, I got ... OK

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

uname -v --kernel-version

```shell
uname -r -s -v
```
TODO: kernel ver?
#1 SMP PREEMPT Sun, 26 Sep 2021 19:36:15 +0000
