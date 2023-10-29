## Manually

```bash
# SUID/SGID owned by root and executable by any user
find / \( -perm -g=s -o -perm -u=s \) -a -user root -type f -perm -o=x -exec ls -ld {} \; 2>/dev/null
```
