# chaojigongshi-xuperchain-othernode

修改 conf/xchain.yaml 文件，添加相应的 bootNodes 节点 netURL

docker run -d --name other -v $PWD/data/blockchain:/home/work/xuperunion/data/blockchain -v $PWD/data/keys:/home/work/xuperunion/data/keys -v $PWD/data/netkeys:/home/work/xuperunion/data/netkeys -v $PWD/conf:/home/work/xuperunion/conf -p 37102:37101 -p 47102:47101 -p 37202:37200 zfq17876911936/chaojigongshi-chain-node:1.0-20201112-nofee

docker run -d --name xchain -v $PWD/data/blockchain:/home/work/xuperunion/data/blockchain -v $PWD/data/keys:/home/work/xuperunion/data/keys -v $PWD/data/netkeys:/home/work/xuperunion/data/netkeys -v $PWD/conf:/home/work/xuperunion/conf -p 37101:37101 -p 47101:47101 -p 37200:37200 zfq17876911936/chaojigongshi-chain-node:1.0-20201112-nofee
