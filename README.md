# CS453 Individual AI Project: Campus Delivery Agent

## Student and task
- **Student ID:** 09211116
- **GitHub:** [MohamedAlMasoudi](https://github.com/MohamedAlMasoudi)
- **Chosen project:** Campus Delivery Agent
- **Assigned variant:** variant 1 (computed by `make_variant` from the student ID)
  - Start: S
  - Goal: F
  - Removed road: B–E

## Project summary
A delivery agent moves on a small campus map modeled as an undirected graph of 8 locations (S, A, B, C, D, E, F, G). The agent must travel from S to F and perform the Deliver action. A state is `(location, delivered)`, every action costs 1, and the goal is reached when `delivered == True`.

The notebook contains:
- **Task 1:** PEAS and environment analysis.
- **Task 2:** state representation, legal actions, transitions, goal test, costs and service (Deliver) rules.
- **Task 4:** a simulator that checks legal moves, applies the Deliver action and rejects illegal actions.
- **Task 5:** BFS (uninformed search) with the assigned mission output.
- **Task 6:** A* (informed search) using the supplied heuristic table, with the assigned mission output.
- **Tasks 10-11:** sources and assistance disclosure, and the submission checklist.

## Files
- `project.ipynb`: the complete project notebook (all code and explanations).
- `README.md`: this file.

## Dependencies
Python 3 (Google Colab default). Only the standard library is used: `copy`, `platform`, `collections`, `heapq`, `itertools`. No extra installs, GPU, paid API or website are needed.

## How to run
1. Open the notebook in Colab: [Open in Colab](https://colab.research.google.com/github/MohamedAlMasoudi/cs453-ai-project/blob/master/project.ipynb)
2. Check that `STUDENT_ID = "09211116"` (a string, leading zero preserved) in the Task 2 cell.
3. Select **Runtime > Restart session and run all**.
4. Expected output: variant 1, goal F, removed edge `('B', 'E')`; simulator tests reject illegal actions; BFS and A* both return a 3-move route S -> A -> C -> F followed by Deliver, and the final state is `('F', True)`.

## Sources and assistance
See Section 10 of the notebook for the full disclosure of the course material and AI assistance used, and how the work was verified.
