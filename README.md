# DOE-CRC Coder
This code is to transfer trajectory/velocity curve (as shown in the upper left corner of the below figure) to a binary code and show the trajectory/velocity information in a electric panel (as shown in the bettom of the below figure). Thus, the panel can help transmit the preceding vehicle's trajectory/velocity to the following vehicle equipeed with a camera. About the algorithm of camera to detect the binary code, please check [e-sign](https://github.com/CATS-Lab/e-sign). 
<div align=center>
<img src="https://user-images.githubusercontent.com/37428219/201544011-bdecb513-c819-45bb-823e-78a237d40909.png" width=400 height=300 />
</div>
The algorithm we use to encode is Cyclic redundancy check (CRC) algorithm. For more information, please check https://zlib.net/crc_v3.txt.
CRC needs a initialize check code. In this project, the default initialize check code is a 8-byte code. 
Input: Discrete trajectory/velocity data. 
Output: CRC_message, CRC_polumial, CRC_divisor, CRC_reminder,  
