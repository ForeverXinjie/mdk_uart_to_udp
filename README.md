# mdk_uart_to_udp
my mdk project：W7500P  Uart to UDP
初始版本说明：
  1.UDP转串口发送是在loopback函数中发送udp数据后插入发送串口数据函数完成
  2.串口收发用中断完成，由于水平有限，未能建立双缓冲或者环形缓冲区。在数据长度不超过一定值时，串口向udp转发数据不丢失。
    但是在数据长度较长或者连续收发文件时，数据丢包量较大。
以上为初始版本说明。
