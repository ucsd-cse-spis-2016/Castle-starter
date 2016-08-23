# Castle-starter

Castle Game starter repo

# HOW TO PLAY

For each remaining day of SPIS, you can play the Castle game by updating the file `castles.json` in this repo
with your entries for that day's competition.

The file `castles.json` should contain the following when you first copy this repo. 

```json

{ "First_L" : 
  { 
    "0822" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0823" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0824" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0825" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0826" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0827" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0828" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0829" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0830" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0831" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0901" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
   }
}
```

To enter each days competition, you'll edit the numbers in the list for that day so that they represent your 10 castles.

The numbers should sum to 100, and should all be non-negative.

To check your numbers, you can run the script `check_castles.py`, either in IDLE,
or by typing `python check_castles.py` at the Unix command line (bash shell prompt).

The script will check the following:

* that your JSON is formatted properly
* that you changed the name from "First_L" to something else
* that the dates are the expected ones
* that your list of castles for each date has exactly 10 castles
* that your lists contain only non-negative integers
* that your lists sum to 100 or less

If the values all pass the test, then you'll be entered into the competition.


