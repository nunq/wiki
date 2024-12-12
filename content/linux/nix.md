# nix

nix shell preamble for python scripts:
```bash
#!/usr/bin/env nix-shell
#!nix-shell -i python3 -p "python3.withPackages(ps: [ ps.tqdm ps.requests ])"

# ... python code
```