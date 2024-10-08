# Should Collaborative Robots be Transparent?

This is a repository for our paper ["Should Collaborative Robots be Transparent?"](link). We include the codes for:
 - The example described in Section 4.3 (`main.py`)
 - 1 DoF simulation in Section 5 (`sim_1d.py`, `sim_1d_bayes.py`, `sim_1d_memory.py`)
 - 2 DoF simulation in Section 5 (`sim_2d.py`, `sim_2d_bayes.py`, `sim_2d_memory.py`)
 - Online user study in Section 6.1 (`userstudy1_parking.py`, `userstudy1_passing.py`, `userstudy1_turing.py`)
 - In-person user study in Section 6.2 (`userstudy2_blocks.py`)
 - To reproduce the figures in the paper use `plotter.py` in sim1 and sim2 folder
 

## Requirements

 - python3
 - numpy
 - matplotlib

## Instructions

Run each code using `python [filename].py` for instance `python main.py`
 - To see arguments available for each code refer to the comments for them. For instance for the `main.py`: 
     - To see optimal behavior that is *fully opaque*, include the argument '--example fully'
     - To see optimal behavior that is *rationally opaque* but not *fully opaque*, use the argument '--example rationally'

## Simulation Results

 - Results for Section 5 codes are stored in sim1 and sim2 folder
 - By choosing different parameters different results can be obtained which are automatically saved in sim1 and sim2
 
## Example Results

Results from running `python.py`

 - *--example fully* | the human's final belief should be 0.0 for each type of robot and each type of human. In other words, the system is fully opaque and the robot's optimal behavior convinces the human that the robot is confused.
 - *--example rationally* | the human's final belief should be 0.0 for capable and confused robots if the human is rational. When the human is *irrational*, the final belief for confused is 0.0 and the final belief for capable is 0.4. By perturbing the system the irrational human uncovers information about the robot's type.

## Online Study Scenes
The following gifs correspond to the three tasks in our online user study: *Passing*, *Parking*, and *Turning*. The gifs include two example behaviors observed during the experiment.
<div style="display: flex; justify-content: center; align-items: center;">
  <img src="https://github.com/user-attachments/assets/9d7e976e-4b9d-44a9-a691-dbfff49aa457" style="width: 200px; height: auto; margin: 0 10px;">
  <img src="https://github.com/user-attachments/assets/fbf0027b-abfc-4b1b-97b8-d01ce8642942" style="width: 200px; height: auto; margin: 0 10px;">
  <img src="https://github.com/user-attachments/assets/0ad20d35-c1c0-4653-a3ee-5086894d0a65" style="width: 200px; height: auto; margin: 0 10px;">
</div>

### Online Study Survey Questions
Below is an image of the user interface. This include instructions, an image of the current state, and a multiple choice menu for the human to select their next action:
<div style="display: flex; justify-content: center; align-items: center;">
  <img src="https://github.com/user-attachments/assets/46fd9d6c-b7c4-4a92-857a-b273c255d71c" style="width: 600px; height: auto; margin: 0 10px;">
</div>

At the end of each interaction, participants answered a question about their subjective perception of the robot partner. This question (and the scale for answering) is shown below:
<div style="display: flex; justify-content: center; align-items: center;">
  <img src="https://github.com/user-attachments/assets/335dc63c-5087-4bdd-b9e9-136ef0e9b3ba" style="width: 600px; height: auto; margin: 0 10px;">
</div>



