# Castle-starter

Castle Game starter repo

# HOW TO PLAY

1. <b>Create `spis16-Castles-`<em>First-L</em> repo</b>: Using [Method 1, with starter code](http://ucsd-cse-spis-2016.github.io/topics/github_create_repo/#method1), create a new private repo with these instructions:

    * Create the repo under the `ucsd-cse-spis-2016` github organization
    * Give it the name `spis16-Castles-First-L` where `First` is your first name, and `L` is the first letter of 
    your last name.
    * Use this repo (the one you are looking at now, i.e. [https://github.com/ucsd-cse-spis-2016/Castle-starter](https://github.com/ucsd-cse-spis-2016/Castle-starter) as the starter code to import)

2.  Use `git clone` to clone that repo into your `~/github` directory.

3.  Use `idle` to edit the `castles.json` file to change the zeros for each day to the 
    numbers you want for your castles (more details below.).   

4.  Run `python check_castles.py` to verify the validity of your castles (i.e. to make sure
    you don't have more than 100 in any given line, etc.)

5.  Use `git push origin master` to update the copy on github.

6.  Each day, return and update your castle values for the next days round.

Note: You can also edit directly  at the github web page.  If you do that, the changes
won't be reflected in the clone unless and until you use `git pull origin master` to update 
the cloned copy from the github.com copy.

# Editing `castles.json` to set your castles

For each remaining day of SPIS, you can play the Castle game by
updating the file `castles.json` in this repo with your entries for
that day's competition.

The file `castles.json` should contain the following when you first copy this repo. 

```json
{ 
    "0823" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0824" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0825" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0826" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0827" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0828" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0829" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0830" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0831" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0901" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ]
}
```

To enter each days competition, you'll edit the numbers in the list
for that day so that they represent your 10 castles.

The numbers should sum to 100, and should all be non-negative.

For example, if Alex Triton were playing, and Alex wanted to be ready
for the competition that ends on 08/23 at midnight, Alex might put
this into the `castles.json` file in
`https://github.com/ucsd-cse-spis-2016/spis16-Castles-Alex-T`:

```json

{ 
    "0823" : [ 11, 11, 11, 11, 22, 5, 6, 21, 1, 1 ],
    "0824" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0825" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0826" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0827" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0828" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0829" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0830" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0831" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ],
    "0901" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ]
}
```

# Checking your numbers for validity

To check your numbers, you can `git clone` the repo you create into your `~/github` directory,
then cd into your repo.

To check that you edited the `castle.json` file correctly, you can run the script `check_castles.py`,
either in IDLE, or by typing `python check_castles.py` at the Unix
command line (bash shell prompt).

The script will check the following:

* that your JSON is formatted properly
* that the dates are the expected ones
* that your list of castles for each date has exactly 10 castles
* that your lists contain only non-negative integers
* that your lists sum to 100 or less

If the values all pass the test, then you'll be entered into the competition.

