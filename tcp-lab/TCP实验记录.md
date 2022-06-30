序列号：每发送一次新的数据包，就累加一次该序列号的大小；

确认应答号：下次期望收到的数据序列号，表示 确认应答号 - 1 的数据包已经被正常接收；

<img src="https://img.wzf2000.top/image/2022/05/11/021801285291106.png" alt="021801285291106" style="zoom:50%;" />

send sequence：

snd_una：最早未确认过的 seq

snd_nxt：下一个将要发送的 seq

snd_wnd：发送窗口大小

snd_wl1：记录最后接收的报文段序号，用于更新发送窗口

snd_wl2：记录最后接收的报文的确认序号，用于更新发送窗口

iss：初始化发送报文段序号

<img src="https://img.wzf2000.top/image/2022/05/11/021800437329324.png" alt="021800437329324" style="zoom:50%;" />

receive sequence：

rcv_nxt：下一个将要接收的 seq

rcv_wnd：接收窗口大小

irs：初始化接收报文段序号

