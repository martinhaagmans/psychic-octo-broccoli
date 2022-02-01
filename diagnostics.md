# Tricks for diagnostics

### Move amplicons data to network
From SERIE/output:
```bash
for i in $(grep GNAS ../SampleSheet.csv | awk -F "," '{print $1}') ;
  do 
    echo $i ;
    cp ${i}/*.ba* /mnt/ngs/SERIE ;
  done ;
```
