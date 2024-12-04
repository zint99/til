# rm failure as device or resource busy

when I wanna rm -rf myDir, log:

```bash
Device or resource busy
```

Reason: There are still process alive

Solution:

1. `lsof +D yourDir`
2. `kill -9 pid`
