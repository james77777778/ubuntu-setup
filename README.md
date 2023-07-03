# Ubuntu Setup

My setup for Ubuntu desktop

## Undervolt

[https://github.com/georgewhewell/undervolt](https://github.com/georgewhewell/undervolt)

```bash
sudo pip install undervolt
sudo cp ./systemd/undervolt.service /etc/systemd/system/undervolt.service

systemctl start undervolt.service
systemctl enable undervolt.service

# check
sudo apt install stress i7z
sudo undervolt --read
sudo i7z
sudo stress -c [num_cpu]  # at another terminal
```
