# tee

ping loop with time:
```bash
ping 172.16.5.9 | while read pong; do echo "$(date +%Y-%m-%d_%H%M%S): $pong" | tee -a orc8r-ping.logs; done
```

