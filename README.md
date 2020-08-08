# hello-code
just try it!
#在GPL平台上下载探针ID&基因名txt文件，直接用excel打开，有的会有空格
#除去空格的代码见下，原理是：现用na.strings把空格变为NA值，然后用na.omit()除去缺失值
a = read.csv("bladder cancer -GEO数据挖掘/实验步骤/8.GPL探针基因名下载/GPL10150.csv",na.strings)
newa = na.omit(a)
write.csv(newa,file = "bladder cancer -GEO数据挖掘/实验步骤/8.GPL探针基因名下载/new_GPL10150.csv")
