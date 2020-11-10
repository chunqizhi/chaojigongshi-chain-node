# chaojigongshi-xuperchain-othernode

mkdir data

将创世区块的相关地址复制到 data 目录下面
cp -r  keys/ netkeys ./data

docker run -d --name xchain -v $PWD/data/blockchain://home/work/xuperunion/data/blockchain -v $PWD/data/keys://home/work/xuperunion/data/keys -v $PWD/data/netkeys://home/work/xuperunion/data/netkeys -v $PWD/conf:/home/work/xuperunion/conf -p 37101:37101 -p 47101:47101 -p 37200:37200 zfq17876911936/chaojigongshi-xuperchain-othernode:1.0-20201110-nofee

