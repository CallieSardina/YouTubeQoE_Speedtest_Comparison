# YouTubeQoE_Speedtest_Comparison

## Get Users for Tcpreplay Based on Throughput Value

## Run Speedtest on Background Traffic 

Set the time to start the Speedtest stats collection in the speedtest() function in [].ipynb. Keep in mind that the raspi nodes are 7 hours ahead.

Run the Speedtest, [].ipynb.

## Run YouTube QoE Session on Background Traffic 

Replay the Traffic with Tcpreplay at specified time, using command `echo tcpreplay [IP address] | at 2:30 PM'.

Set the time to start the YouTube QoE stats collection in the debug_watch() function in [].ipynb. Keep in mind that the raspi nodes are 7 hours ahead.

Run the YouTube QoE collection, [].ipynb.
