# PeerToCP Benchmarking Result

Result is visualized in the [PeerToCP Benchmarking Notebook](benchmark-vis.ipynb). 

## Replicating The Benchmark

Make sure you read on how to do the test on the [main repository](https://github.com/hockyy/peertocp). The test will result in several logs that will be available in the `./out` repository. Resource benchmarking uses the netdata. But you can replace this with other benchmarking tool. If you use netdata, the fetch command will more or less looks like the followings. Modification must be made to adjust it to your own environment.

```bash

netd () {
	curl "http://$1:19999/api/v1/data?chart=apps.mem&dimension=node&after=$2&points=0&group=average&gtime=0&timeout=0&format=csv&options=seconds" > mem-$3.csv
	curl "http://$1:19999/api/v1/data?chart=system.ip&after=$2&points=0&group=average&gtime=0&timeout=0&format=csv&options=seconds" > network-$3.csv
	curl "http://$1:19999/api/v1/data?chart=apps.cpu&dimension=node&after=$2&points=0&group=average&gtime=0&timeout=0&format=csv&options=seconds" > cpu-$3.csv
}

scpd () {
	scp -r hocky@$1:~/peertocpnext/out/ ./$2
}
```

