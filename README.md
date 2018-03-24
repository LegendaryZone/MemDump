# MemDump

**Android memory dump**

```bash
adb push memdump /data/local/tmp/
adb shell
  su
  chmod 0777 /data/local/tmp/memdump
  /data/local/tmp/memdump - $(PID) 0x6B32B000 0x6B32C000 - /data/local/tmp/dump.data
  /data/local/tmp/memdump - $(PID) 1798483968 1798488064 - /data/local/tmp/dump.data
adb pull /data/local/tmp/dump.data
```
