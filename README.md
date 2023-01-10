# How to run
```
git clone https://github.com/Adjuntor/program-kun.git
cd program-kun
pip install --no-cache-dir -r requirements.txt
```
Edit the config.py with the correct values.
```
python3 main.py
```

# Docker Image
Requires docker to be installed.
```
git clone https://github.com/Adjuntor/program-kun.git
cd program-kun
```
Edit the config.py with the correct values.
```
docker build -t program-kun .
docker run -d --name=program-kun --restart=always program-kun 
```

# Delete Docker Container
```
docker stop program-kun
docker rm program-kun
```

# Updating
To update the bot use the command below to ignore updating the config.py, keeping your local version.
```
git update-index --skip-worktree config.py
```
and just do an update.
```
git pull
```
