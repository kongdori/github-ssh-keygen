## 참고
* https://www.lainyzine.com/ko/article/creating-ssh-key-for-github/

***

## 1. ssh-keygen
  ```bash
  # ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
  ssh-keygen -t ed25519 -C "your_email@example.com"
  ```

***

## 2. ~/.ssh/config
  ```vim
  Host github.com
    # IdentityFile ~/.ssh/id_rsa
    IdentityFile ~/.ssh/id_ed25519
    User git
  ```

***

## 3. github 설정
1. Your Setting
2. SSH and GPG keys
3. New SSH Key
4. id_ed25519.pub (id_rsa.pub) 복사

***

## test
```
ssh -T git@github.com
```

