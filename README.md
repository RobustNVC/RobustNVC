# RobustNVC
A Vision-Transformer-based neural video codec that is robust to network packet losses. 

It achieves superior loss resilience performance than [Grace](https://github.com/UChi-JCL/Grace/tree/master)(NSDI 2024) and [DCVC-DC](https://github.com/microsoft/DCVC/tree/main/DCVC-DC) (CVPR 2023).

Inference examples with `50% packet loss` of `RobustNVC` and `DCVC-DC` (with and without retransmission) under the same network bandwidth and transmission time (`RTX` means retransmission and `RTT` means network round-trip time ):


| Original | DCVC-DC(w/o RTX) | DCVC-DC(RTX, RTT=10) |RobustNVC(w/o RTX) |
|----------|----------|----------|----------|
| ![Alt text](images/bee_original_im016_crop.png) | ![Alt text](images/dcvc-im016-bee.png) | ![Alt text](images/dcvc-dc-im016-bee-rtt10_crop.png) | ![Alt text](images/bee_10_drop5_frame16.png) |
| ![Alt text](images/dog-original_im016_crop.png) | ![Alt text](images/dcvc-im016-dog.png) | ![Alt text](images/dcvc-dc-im016-dog-rtt10_crop.png) | ![Alt text](images/dog_10_drop5_frame16.png) |
| ![Alt text](images/boat_original_im016_crop.png) | ![Alt text](images/dcvc-im016-boat.png) | ![Alt text](images/dcvc-dc-im016-boat-rtt10_crop.png) | ![Alt text](images/boat_10_drop5_frame16.png) |

## Check out later for updates!
