- Used the commands below to initialize the GIT Repo
```
mkdir MarketPeak_Ecommerce
cd MarketPeak_Ecommerce
git init
```

- Downloaded the ECommerce template from Tooplate website

- Copied the template into my project folder using:
```
cp -a <source> <destination>
```

- Staged and committed the template to Git using:
```
git add .
git config --global user.name "YourUsername"
git config --global user.email "youremail@example.com"
git commit -m "Initial commit with basic e-commerce site structure"

```

- Pushed the changes to Git using:
```
git remote add origin https://github.com/your-git-username/MarketPeak_Ecommerce.git
git push -u origin main

```

- Setup an EC2 instance and connected to it

- Cloned the repo to the linux server using SSH:
Used the ssh-keygen command to generate public/private key pair
Used the cat /home/ubuntu/.ssh/id_rsa.pub command to display and copy the public key and added it to my github

- Cloned the repo using:
```
git clone git@github.com:yourusername/MarketPeak_Ecommerce.git
```

- Installed Apache webserver using:
```
sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
```

- Cleared the apache server folder and copied the ecommerce files into it using:
```
sudo rm -rf /var/www/html/*
sudo cp -r ~/MarketPeak_Ecommerce/* /var/www/html/
```

- Reloaded the server using:
```
sudo systemctl reload httpd
```

- Implemented continuous integration and depllyment by:
Creating a development branch
Pushing new features to that branch
Reloading the http server each time

