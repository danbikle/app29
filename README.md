
# ~/app29/README.md

This repo contains some demos which I wrote to connect my mind to the convnet.js API.

To get started I did this:

```bash
cd ~
git clone https://github.com/karpathy/convnetjs.git cnet

cd ~
git clone https://github.com/danbikle/app29.git
cd ~/app29
git checkout -b mybranch
cat ~/cnet/src/*.js > convnet.js
```

I wanted to use a Node.js web server to serve convnet.js to my browser.

I installed Node.js into my home folder like this:

```bash
cd ~
rm -rf node
rm -rf node-v5.0.0-linux-x64
rm  -f node-v5.0.0-linux-x64.tar.gz

wget https://nodejs.org/dist/v5.0.0/node-v5.0.0-linux-x64.tar.gz
tar zxf node-v5.0.0-linux-x64.tar.gz
mv node-v5.0.0-linux-x64 node

export       PATH="${HOME}/node/bin:${PATH}"
echo 'export PATH="${HOME}/node/bin:${PATH}"' >> ~/.bashrc
```

Next I installed the web server package into my copy of Node.js:

```bash
cd ~/app29
npm install
```

I did not need to specify the name of the package because the name was already inside package.json which is where npm will look.


