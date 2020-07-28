# EQP Loves Tennis :tennis:

## Coding Exercise

Write a .NET web application that can track the score of a Wimbledon Men’s Singles tennis match:
- The main class should have three accessible methods playerAWonPoint(), playerBWonPoint(), currentScore()
  - currentScore() should return a String of the form `<Player A sets>/<Player B sets> <Player A games>/<Player B games> <Player A points>/<Player B points>`
  - For example, `2/1 3/2 AD/40` indicating that Player A is 2 sets to 1 up, Player A is 3 games to 2 up in the fourth set, and has Advantage in the current game
  - Another example, `2/1 6/6 5/3` indicating that Player A is 2 sets to 1 up, it is 6 all in the fourth set and Player A is leading the tie break 5-3
  
You are free to verify your program however you see fit.

### How to submit
Send us a link to a private GitHub repository containing your solution. Ideally, we would like to avoid having public solutions so please keep the repository private and add us [@eqpaymaster](https://github.com/eqpaymaster) as a collaborator so that we can see your code.

### Guidance notes
- Most people spend about 2 hours on this exercise, though there’s no time limit. Incomplete solutions will not be penalised, although the program should execute successfully

## Appendix
### The rules of Tennis

- To win the tennis match a player must win three sets
- To win a set, a player must win six games and be at least two games ahead of their opponent
- To win a game, a player must win four points and be at least two points ahead of their opponent
- In any of the first four sets, if the score reaches six games all, a tie break is played to decide who wins the next game and thus the set
- In the fifth set, if the score reaches twelve games all, a tie break is played to decide who wins the next game and thus the set and match
- To win a tie break, a player must win at least seven points and be at least two points ahead of their opponent
- When declaring the score of the match, you list the numbers of sets each player has, followed by the number of games in the current set, followed by the number of points in the current game
- Having 0, 1, 2 or 3 points in a game is declared as 0, 15, 30 and 40 respectively.

### Example:
- Player A wins the first point - score is 15/0
- Player B wins the next point - score is 15/15
- Player B wins the next point - score is 15/30
- Player A wins the next point - score is 30/30
- Player B wins the next point - score is 30/40
- Player A wins the next point - score is 40/40
- Player A wins the next point - score is AD/40
- Player B wins the next point - score is 40/40
- Player A wins the next point - score is AD/40
- Player A wins the next point - game to Player A

See https://en.wikipedia.org/wiki/Tennis_scoring_system for reference
