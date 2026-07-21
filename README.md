# Cloud EC2 Lab

This repository contains a simple static webpage for an AWS EC2 hosting lab.

## Steps to host on AWS EC2

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
