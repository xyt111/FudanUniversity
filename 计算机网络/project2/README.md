project2</br>
====
实现了全部功能，进行了拥塞处理，包括慢启动、超时重传、快速重传</br>
</br>
个人增加的文件：</br>
=
queue.c/h：队列数据结构的封装文件并实现了队列的一系列操作的函数</br>
task.c/h：上传和下载任务的函数分装文件，定义了任务、连接等结构，实现了对上传和下载的控制操作函数</br>
timer.c/h：计算时间辅助文件，实现了计算两个时间的差、设定时间等函数</br>
transfer.c/h:传送和文件处理的函数封装文件，实现了传送过程中对接收数据、文件的处理函数，以及发送数据包函数</br>
udpPacket.c/h：数据包类型的定义封装文件，实现了不同类型数据包的生成函数以及网络、本地类型转换的辅助函数</br>

原本就有的文件：</br>
=
peer.c:程序的主结构，主函数入口，实现了对用户输入命令的处理和以及对接收到的不同类型数据包处理</br>
bt_parse.c/h：用于解析用户输入的参数，读取文件生成peer的信息，提供打印peer信息的函数</br>
chunk.c/h：chunk文件相关函数，用于生成文件的哈希值，并提供十六进制与二进制的转化</br>
debug.c/h：用于调试的程序，输出调试信息</br>
input_buffuer.c/h:处理用户的输入程序</br>
sha.c/h：哈希函数文件，封装了特定哈希函数</br>
spiffy.c/h：传输与接收数据的接口，实现了发送和接收数据的函数。</br>