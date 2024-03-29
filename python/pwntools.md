# pwntools

python package to automate socket interaction

## install:

`python3 -m pip install --user pwntools`

## Example

```python3
from pwn import remote
r = remote('0.cloud.chals.io', 16992)

s = r.recvuntil('Speak thy new password:').decode('ascii')
print(s)
r.send('abc123\n'.encode('ascii'))
r.interactive()
```
