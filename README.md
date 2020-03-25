# TIC-TAC-TOE

*Objectives: 
- Computer to get optimal solution against the human 
- Use Minimax algorithm to make decisions of each moves

*Agent Description 
1. Computer agent 
Computer gets either to make a move first or second. Then it uses Mini-max algorithm to make optimal moves so that it could stop human player to not win and to win itself. This algorithm is a recursive or backtracking algorithm which is used in decision making. The Mini-max algorithm performs depth-first search algorithm for exploration of the complete game tree. 
The PEAS description for the agent are: 
Performance measure: Win, lose or draw 
Environment: 3x3 grid Actuators: set_move function to make a move 
Sensors: moves from human 

2. Human agent 
Similarly, Human player makes either first or second move. Then it tries to win the game or tries to block the Computer from winning the game. 
The PEAS description for the agent are: 
Performance measure: Win, lose or draw. 
Environment: 3x3 grid 
Actuators: number key pad 
Sensors: game screen

*Agent Environment

The game environment is represented in 3x3 grid. The two players are represented by X or O. Each player will place their respective sign on the grid to get one’s solution. A player can win if it has its sign over one row or on column or in any diagonal way.
Some of the properties of the task environment that this game fits in are

1.Observable: If an agent’s sensors give it access to the complete state of the environment at each point in time, then we say that the task environment is fully observable. Here agent’s sensors does give the access to the complete state of environment which is 3x3 grid, hence making it fully observable.

2.Deterministic: If the next state of the environment is completely determined by the current state and the action executed by the agent, then we say the environment is deterministic. If the environment is deterministic except for the actions of other agents, we say the environment is Strategic. Here the next state of the grid is completely dependent of the action taken in previous states hence making it as an Strategic.

3.Episodic: In sequential environment, the current decision could affect all future decisions. In this game also, every possible moves has their own possible future impact hence making it sequential.

4.Static: If the environment can change when as agent is deliberating, then we say the environment is dynamic. If the environment itself doesn’t change with the passage of time but the agent’s performance score does, then we say the environment is semi-dynamic.

5.Discrete: The game has finite number of distinct states. It also has a discrete set of percepts and actions. So it has discrete environment.

6.Agents: The agent playing tic-tac-toe is a two-agent environment. In this game the opponent entity (Human or computer) trying to maximize its performance measure, which by the rules of the game, minimizes another agent’s performance.
