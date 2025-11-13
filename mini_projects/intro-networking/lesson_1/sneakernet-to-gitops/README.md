## Stage 1: Sneakernet
- Manual copy: `cp sneakernet/hello.txt production-sim/hello-deployed.txt`
- No automation
- No audit trail
- Human error risk
- Not repeatable

## Stage 2: BBS (LAN File Server)
- Server: `python3 -m http.server 8000`
- Client: `curl http://IP:8000/hello.txt`
- Uses **network** — no USB
- Still manual trigger
- No version control