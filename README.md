# YouTubeQoE_Speedtest_Comparison

## Get Users for Tcpreplay Based on Throughput Value

Run getDataRate.py with the desired throughput value. Access to this Python file is only available to those on the server, permissions are necessary. Please contact the authors for further information.

On the upstream server and the downstream server, run Tcpreplay on the pcap files associated with the resultant IP address from above. To ensure that both of these servers begin replaying the netwrok traffic simultaneously, `echo [CMD] | at [TIME]' can be used. 

Run the background traffic for the duration of the data collection tasks.

## Run Speedtest on Background Traffic 

Set the time to start the Speedtest stats collection in the speedtest() function in speedtest.ipynb. Keep in mind that the raspi nodes are 7 hours ahead.

Run the Speedtest, speedtest.ipynb.

The results will be printed to standard output. Save them in a text file.

## Run YouTube QoE Session on Background Traffic 

Replay the Traffic with Tcpreplay at specified time, using command `echo tcpreplay [IP address] | at 2:30 PM'.

Set the time to start the YouTube QoE stats collection in the debug_watch() function in youtube_qoe.ipynb. Keep in mind that the raspi nodes are 7 hours ahead.

Run the YouTube QoE collection, youtube_qoe.ipynb.

The resultant text file with the Stats for Nerds will be sent to your configured Google Storage Bucket.

## Visualization and Analysis

Use QoE_Speedtest_Analysis.ipynb to viualize the Speedtest and YouTube Stats for Nerds results. To do this, replace the filepaths with the respective filepaths to the two text files from above.
