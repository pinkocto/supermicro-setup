# supermicro-setup
supermicro server setup-guide

- Connect to the internet: `Use wired connection`
- What do you want to do with Ubuntu?: `install Ubuntu`
- How would you like to install Ubunto?: `Interactive installation`
- What apps would you like to install to start with?: `Default selection`
- How do you want to install Ubunto?: `Erase disk and install Ubuntu` (Advanced 
- 

```python
# 아래 코드를 실행하기 전 네트워크 설정 먼저
# 우측 상단 네트워크 모양 > 톱니바퀴 > Ethernet >  IPv4 > Manual (Addresses, DNS 입력) > Apply
# 네트워크가 잘 연결 되었으면 터미널을 열고 아래의 코드를 입력한다.
sudo apt update
sudo apt install openssh-server
```
