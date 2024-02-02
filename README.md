This assignment aims to help you practice the heap data structure and heap sort algorithm. Your 
main task in this assignment is to develop a simple leaderboard system using C programming 
language.

OVERVIEW

Every leaderboard needs a couple of sorting features to help you see which participant is the leader 
when it comes to a certain aspect. Having the most wins does not mean the best win rate, and the 
expectation to win placed upon each opponent plays a major role, especially in the betting 
department. Since heap sort has been the highlight of the week, the focus will mostly be on 
implementing it to sort our leaderboard the way the user desires.
In this assignment, you will develop a leaderboard system for an online battle arena video game 
which supports the following functionalities:

1. Read a data file containing the names of every champion and how much people bet in their 
favor, which for the sake of simplicity, we will consider to be their expected win rate.
2. Read a data file containing information about every battle that took place between said 
champions. The information is basically the identity of the participants and who won.
3. Sort or rank every champion based on either their expected win rate, actual win rate, or
expectation skew.
4. Print the results of the sort with the respective information.

INPUT

The program will have three inputs:
 Sorting criteria: (1) actual win rate, (2) expected win rate, or (3) expectation skew.
 Champion Data: A file will contain the names of every champion and their expected win rate
separated by a space (i.e., championName expectedWinRate) in which each line will 
correspond to a different champion. Do not make any assumptions about the number of 
champions. championName can have maximum 50 characters without any space.
 Battles’ Data: A distinct file will contain information about every battle that took place 
between these champions. Each line represents a separate battle and every piece of 
information in a line is separated by a space (i.e., battleID battleParticipant1 
battleParticipant2 winner).
This program takes these inputs them as command-line arguments as follows:
leaderboardMaker sortingCriteria ChampionDataFile BattlesDataFile
 leaderboardMaker: When you run your program from the command line, you need start with 
its name. The name of the compiled program will be leaderboardMaker.
 sortingCriteria: This should be an integer value – 1 for actual win rate, 2 for expected win rate, 
and 3 for expectation skew.
 ChampionDataFile: This is the name of the file containing the names of the champions and 
their expected win rates.
 BattlesDataFile: This is the name of the file containing the battles' information
An example is provided below:
leaderboardMaker 1 champions.txt battles.txt
