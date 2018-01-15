此代码库修改自https://github.com/hyperledger/fabric-samples，请确保运行环境中已安装node(v6.11.0或以上)和npm(3.10.10或以上)。

安装流程：

假设读者运行环境已安装golang，并且正确设置GOPATH。

i.	下载本代码库
cd $GOPATH/src
git clone https://github.com/LordGoodman/fabric-samples.git

ii.	下载Fabric常用工具集
cd ~/Downloads
$ curl https://nexus.hyperledger.org/content/repositories/releases/org/hyperledger/fabric/hyperledger-fabric/linux-amd64-1.0.0/hyperledger-fabric-linux-amd64-1.0.0.tar.gz | tar xz

iii.	把工具集加入到PATH环境变量中
echo 'export PATH=$PATH:$HOME/Downloads/bin' >> ~/.profile
source ~/.profile

iv.	下载Fabric的docker镜像
cd $GOPATH/src/fabric-samples/scripts && bash fabric-preload.sh
