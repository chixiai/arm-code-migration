# arm-code-migration

在命令行上创建新的存储库
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/chixiai/arm-code-migration.git
git push -u origin main

从命令行推送现有存储库
git remote add origin https://github.com/chixiai/arm-code-migration.git
git branch -M main
git push -u origin main

从其他存储库导入代码

交叉编译器：
下载：https://releases.linaro.org/components/toolchain/binaries/4.9-2017.01/arm-linux-gnueabihf/
    gcc-linaro-4.9.4-2017.01-x86_64_arm-linux-gnueabihf.tar.xz
安装：sudo mkdir /usr/local/arm
    sudo cp gcc-linaro-4.9.4-2017.01-x86_64_arm-linux-gnueabihf.tar.xz /usr/local/arm/ -f
    sudo tar -vxf gcc-linaro-4.9.4-2017.01-x86_64_arm-linux-gnueabihf.tar.xz
环境变量：
    sudo vi /etc/profile
    最后面添加 export PATH=$PATH:/usr/local/arm/gcc-linaro-4.9.4-2017.01-x86_64_arm-linux-gnueabihf/bin
安装库：
    sudo apt-get install lsb-core lib32stdc++6
验证：
    arm-linux-gnueabihf-gcc -v










