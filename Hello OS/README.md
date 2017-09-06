# Hello,OS!
采用U盘以及小型虚拟机如同bochsrc运行本实例均可，这里利用后者，根据以下步骤配置：
1.利用bochsrc自带工具创立一个虚拟软盘，终端命令如下
```
bximiage
```
询问创建类型的时候键入fd

2.配置文件bochsrc.txt，使其能够正常挂载a.img软盘

3.利用nasm编译boot.asm
‘’‘
nasm boot.asm -o boot.bin
’‘’

4.根据配置文件运行虚拟机
```
bochs -f bochsrc.txt
```

这样就可以观察到红色的Hello，OS了。
