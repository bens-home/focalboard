# focalboard
My docker-compose setup for FocalBoard


## Getting Started
Make a new folder called `data` and chown it to `nobody`

```
mkdir data
sudo chown -R nobody data
```

Run the compose

```
docker-compose up
```

You are now running focalboard on port `4280`

## Firewall

Allow focalboard through the firewall on your machine. For Ubuntu with `ufw` you can do: 

```
sudo ufw allow 4280/tcp comment "focalboard front end"
```