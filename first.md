一、原码、反码、补码（二进制最高位为符号位）  
位运算基于二进制，包含有原码、反码和补码，计算机内部使用补码表示二进制  
原码：即原二进制，如4对应00 00 01 00;正数反码即时原码，负数反码为原码按位取反，如4对应11 11 10 11;补码：正数补码依然为原码，负数为反码+1，  
即4对应：11 11 10 01  
二、位操作  
~代表把对应数字的补码中的0和1原为取反，这里注意符号位也会取反。如-4对用的原码为：10 00 01 00，对其取~后表示为：01 11 10 10  
三.二进制完全按位置操作，如&，只有位数同位1，取&才为1，如|同样的到理  
四、按位作异或操作，这里可以理解为相同的位操作后都为0，不同的操作后取1  
五、左移和右移。  
左移<<，如00 00 11 00<<3对应01 10 00 00  
右移>>同理，如00 00 11 00>>3对应00 00 00 01  
六.快速计算乘法:  
n<<1对应十进制中的n*2;n>>1对应n/2;n<<m对应n*(2^m);n>>m对应n/(2^m)  
1 << n对应2^n  
a&(-a)可以获得最后为1位置的正数  
python的负数取反码需要进行以下操作：为了获得负数（十进制表示）的补码，需要手动将其和十六进制数0xffffffff进行按位与操作，  
再交给bin()进行输出，得到的才是负数的补码表示  
作业打卡结果如下：  
!(https://github.com/GUESSWIN/python_learn/blob/master/%E6%89%93%E5%8D%A11.png?raw=true)