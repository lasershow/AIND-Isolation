# Evaluate the performance of the heuristic

For each of your three custom heuristic functions, evaluate the performance of the heuristic using the included tournament.py script. Then write up a brief summary of your results, describing the performance of the agent using the different heuristic functions verbally and using appropriate visualizations.

## rubric

`Have at least three (3) evaluation heuristics besides null_score(), open_move_score(), and improved_score() been implemented and analyzed?`

At least three evaluation functions are implemented and analyzed.

`Has the performance of agents against the testing agents been adequately described?`

A brief report lists (using a table and any appropriate visualizations) and verbally describes the performance of agents using the implemented evaluation functions. Performance data includes results from tournament.py comparing (at a minimum) the best performing student heuristic against the ID_Improved agent.

`Does the report make a recommendation about the best evaluation function, and is this recommendation adequately justified?`

The report makes a recommendation about which evaluation function should be used and justifies the recommendation with at least three reasons supported by the data.

## Visualizations

`python tournament.py`

This script evaluates the performance of the custom_score evaluation
function against a baseline agent using alpha-beta search and iterative
deepening (ID) called `AB_Improved`. The three `AB_Custom` agents use
ID and alpha-beta search with the custom_score functions defined in
game_agent.py.

                        *************************
                             Playing Matches
                        *************************

[![https://diveintocode.gyazo.com/a7d544cfe698487f9caa07e7c0b0dfa2](https://t.gyazo.com/teams/diveintocode/a7d544cfe698487f9caa07e7c0b0dfa2.png)](https://diveintocode.gyazo.com/a7d544cfe698487f9caa07e7c0b0dfa2)

Your agents forfeited 249.0 games while there were still legal moves available to play.

## custom_score

The custom_score function is a function inspired by AB_Improved.
This function is a function weighted from the point of view that IsolationGame weights more importantly to restrict the movement of the opponent player rather than simply adding the number that can move to the players.

## custom_score_2,custom_score_3

This function guides you to a location that you can select to AB_Improved, where the other party is not selectable. It aims to obtain new indices by adding self or the range where the other party can select.

## Which evaluation function should be use

I came to the conclusion that costom_function should be used from the result of tournament.py.The main reasons are as follows.

①AB_Custom_2 AB_Custom_3 is strong in a certain field, but it is not guiding overall good performance.

②AB_Custom demonstrates its strength in many fields compared to AB_Improved

③AB_Custom is as simple as AB_Improved
