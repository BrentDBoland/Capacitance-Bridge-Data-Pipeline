This program performs the following operations.


1) Reads a .txt file with the following headers(column labels) and sub-headers(units):

|Freq.|Cap.|Loss|Voltage|Time|
|---|---|---|---|---|
|Hz|pF|tan d|V|

2) converts the MM-DD-YYYY-hh:mm:ss time value to seconds relative to the first measurement.
3) Computes the average values and standard deviation for each frequency.
4) Calculates the real, imaginary, and magnitude impedance from the average values along with error propagated from the std.
5) Scales impedance values for improved fitting and data analysis.
6) Outputs a new file with analyzed appended to the original file name in the designated folder. The new file will have the following headers and sub-headers(units):

|Freq.|omega|Cap. av.|Cap. std|Loss av.|Loss std|ReZ av.|ReZ std|ImZ av.|ImZ std|MagZ av.|MagZ std|ReZ av. 10^-7|ReZ std 10^-7|ImZ av. 10^-7|ImZ std 10^-7|MagZ av. 10^-7|MagZ std 10^-7|Time av.|Time std|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|Hz|rad/s|F|F|tan d| tan d| Ohms|Ohms|Ohms|Ohms|Ohms|Ohms|Ohms 10^-7|Ohms 10^-7|Ohms 10^-7|Ohms 10^-7|Ohms 10^-7|Ohms 10^-7|s|s|
