# Chosing the 200 US Mixed Medley Relay Team
Optimal Assigments Use Case - Min Cost Flow

## Background
In the 2020, the Summer Olympics introduced a new event, the mixed 4 × 100 metre medley relay.  In this event, each team has two male and two female swimmers. Each team decides whether a man or a woman will swim a specific stroke, which means men versus women is possible in a specific stroke, as happened in heats and in finals. Strokes order are in the same order as in a traditional medley race–backstroke, breaststroke, butterfly and freestyle.


The American team finished a disappointing 5th in the race.  My hypothesis was the we did not field the fastest possible team we could based on the swimmers we had available.  This excercise was to determin if there was a faster combination that could have performed better using tools from operations research.


## Aproach

The team assignment is being modeled as a [minimum-cost flow problem](https://en.wikipedia.org/wiki/Minimum-cost_flow_problem) where we are attempting to minimize the expected time to complete the race subject to the constraints imposed by the format, including:

* All strokes (freestyle, backstroke, breaststroke, and butterfly) must be completed
* A swimmer can not be used more than once in the race
* 2 swimmers per gender must participate

Note: data for swim team members was based on results from the US Olympic trials.