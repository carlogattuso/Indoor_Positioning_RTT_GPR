The headers (right to left) of the files in this folder are the following:
- Batch number: The sampling might be splitted in several batches. In our case, there is only one batch, so this parameter can be skipped.
- Actual distance: The real distance between the access point and the android phone. 
- Estimated distance: The estimated distance. This figure involves 7 RTTs (at most) taken by the Android phone, so it is a kind of average.
- Estimation error: It is the error of the distance estimation
- RSS: It is the received signal strength in dBm
- RSS error: It is always 0, since the Android API doesn't provide such figure. 
- Number of RTT samples used for a single distance estimation. This value should be 7 if everything was right, but it can be lower if there is any issue (e.g. mobile at the edge of the coverage area)
- Number of RTT run for a single distance estimation. This value is always 8.
