Fdata
============
Copyright (c) 2023-2043 shanshuyida Technology Co., Ltd. and/or its Affiliates
============
This software is designed for file transsmission in long-range transmission on WAN with maximum 100 Gigabit speed.
It's has all undergone on-site network testing on OTN/MPLS/SD-WAN with 1/10/25/100 Gigabit speed.
============

# iperf3 100Gbps test
## run on server end
iperf3 -s -p 5201 & iperf3 -s -p 5202 & iperf3 -s -p 5203 & iperf3 -s -p 5204

## run on client end
iperf3 -c ip_addr -t 10 -p 5201 & iperf3 -c ip_addr -t 10 -p 5202 & iperf3 -c ip_addr -t 10 -p 5203 & iperf3 -c ip_addr -t 10 -p 5204

![image](https://github.com/user-attachments/assets/76c777f6-a96f-4218-8852-340b98e64791)
##

# RDMA 100Gbps test
## run on server end
ib_write_bw -d fdata -s 4M -q 4 --report_gbits --run_infinitely -R

## run on client end
ib_write_bw -d fdata -s 4M -q 4 --report_gbits --run_infinitely -R ip_addr

![image](https://github.com/user-attachments/assets/f30adce6-21d7-4b8d-8fdb-3e0ac868759b)
##

## More details
### You can get test details through the following links
- https://mp.weixin.qq.com/s/oI_pHtfX_f3Pt2hjzcA6qA
- https://mp.weixin.qq.com/s/pPFif1BnKLqEUISEQvJJUw


### If you want to get more details about fdata, please contact us: 
- wechat: tutudezhenshen
- Tel: 181-2363-6905
- E-mail: shanshuyida@yeah.net
