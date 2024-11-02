# Boat game: cannibal and missionaries boat problem
## A small project from " Introduce to AI " subject
### Problem:
There are 3 missionaries and 3 cannibal on the left bank of a river, together with a boat that can carry 1 or 2 people. If there are more devils than missionaries on one bank, the cannibal will eat the missionaries. Find a way to get them all to the other bank (right side) so that the number of people is not less than the number of devils on the same bank (left or right side), that is, no one is eaten. Let pa, b, kq with 0 ď a, b ď 3 , where a is the number of people, b is the number of devils on the left bank, k “ 1 if the boat is on the left and k “ 0 if the boat is on the right. Then, no state of the problem is clearly defined as follows: • The initial state is (3, 3, 1).
• The boat crosses the river with 1 person, or 1 demon, or 1 person and 1 demon, or 2 people, or 2 demons – the transitions from one state to another are: (1, 0), (0, 1), (1, 1), (2, 0), (0, 2) (where px, yq are the number of people and demons moving from the left bank to the right bank or vice versa).
• The final state is (0, 0, 0).

### How to use
- First, install requirement libraries .
  '''
  Pip install -r requirements.txt
  '''
- The given code had the graph to use (state_space_x) but if you want to generate other graph, go to terminal and type:
  '''
  python generate_full_space_tree.py -d x
  ###With x is height of the tree
  '''
- Solve problems:
  '''
  ##With BFS
  python main.py -m bfs
  ##With DFS
  python main.py -m dfs
  '''
  The main.py will return you  each step to solve and return a png solve file
  Optional you can return png with legend
  '''
  ## DFS with legend
  python main.py -m dfs -l True
  '''
  
