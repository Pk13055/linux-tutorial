# Plan

## Overall Steps

- [wsl](https://learn.microsoft.com/en-us/windows/wsl/install)
- [linux &amp; vim](https://www.loom.com/share/bb4f66d9b2b440fd8e2ef7dcabd540cd?sid=ed3e6188-40c9-438d-8694-df3ee7a376cd)
- python3
    - [install](https://medium.com/@rhdzmota/python-development-on-the-windows-subsystem-for-linux-wsl-17a0fa1839d)
    - [learn](https://youtube.com/playlist?list=PL6gx4Cwl9DGAcbMi1sH6oAMk4JHw91mC_)
- [install docker in wsl](https://docs.docker.com/desktop/wsl/)

- data science
    - [notebook](https://github.com/Synalytica/stock-xyz-research/blob/3723e7726fd8903642ea291831a69fa36c92c1ea/src/research/feature-processing.ipynb)
    - [tutorial](https://youtube.com/playlist?list=PLWKjhJtqVAblQe2CCWqV4Zy3LY01Z8aF1)

## Tutorials

### Tutorial - 1

- You are given a json file called `master.json`
- Convert it to a csv with the following format (for eg):

```csv
timestamp,symbol,open,high,low,close
<YYYY-MM-DD>T<HH:MM:SS>,BTCUSDT,4234,34535,6456,45676
...
```

Make sure you enumerate your steps in the process and what commands you used.


#### Steps


1 - We need to open the master.json file in our terminal ( cat master.json)

2- We need to use grep to extract the only information we need ( symbol , open , high , low , close , timestamp ) - ( grep -E 'symbol|open|close|high|low|timestamp' master.json > output.txt )

3- We can run the output and check for multiple words using the grep combined with the pipe command (|)

4 -We need to store the output in another file using the > symbol (output.txt) 

5 -We can now convert the file to a csv file , by copying the file output.txt to output.csv in the same folder using the cp command

6- We can verify this by opening the csv file using (cat)

Commands used - (ls , cd , cat , grep , > )

