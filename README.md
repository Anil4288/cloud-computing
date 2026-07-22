# Cloud EC2 Lab

This repository contains a simple static webpage for an AWS EC2 hosting lab.
![Hime page](https://github.com/Anil4288/cloud-computing/blob/5362a4abb499e6d1bc8260413e1a0ffef49e3c17/image/Screenshot%202026-07-21%20222049.png)
![homepage](https://github.com/Anil4288/cloud-computing/blob/77a013800f330f71c128a3fe86c1d9118800930d/image/Screenshot%202026-07-21%20222144.png)
![last](https://github.com/Anil4288/cloud-computing/blob/770b2a5001836aeac6faee42492434e1b1c4211a/image/Screenshot%202026-07-21%20222232.png)## Steps to host on AWS EC2

1. Launch an Amazon Linux EC2 instance.
2. Connect to the instance via SSH.
3. Install Apache:

```bash
sudo dnf update -y
sudo dnf install httpd -y
```

4. Start and enable Apache:

```bash
sudo systemctl enable httpd
sudo systemctl start httpd
```

5. Copy the project files into the web root:

```bash
sudo cp -r . /var/www/html/
```

6. Restart Apache:

```bash
sudo systemctl restart httpd
```

7. Open the public IP of the EC2 instance in your browser.
