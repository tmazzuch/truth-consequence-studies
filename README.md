# The role of consequence in evaluating claims as true or false

This folder contains the experiment code for these studies:
- Pilot Study 1
- Pilot Study 2 
- Supplementary Study 1
- Pilot Study 3
- Study 3

## Viewing the studies as a participant

To view these studies, open the file in this folder called `index.html` in your web browser. Then follow instructions from there.

## Viewing the code for the studies

To view the code for each study, navigate to the appropriate code folder (e.g., `s6_code`). Each of these code folders follows the same core structure, as outline below:

| Name | Description |
| --- | --- |
| `index.html` | The wrapper file around the experiment code. Loads `jspsych` plugins and CSS stylesheet, then runs the main experiment files: `conditions.js`, `stimuli.js`, and `experiment.js`. |
| `jspsych` | A directory containing the jsPsych distribution used for this experiment. |
| `experiment.js` | The main logic behind the experiment. Defines a variety of jsPsych routines, such as the consent form, Prolific ID input, and main experiment loop. Combines these routines into the experiment flow. Keeps track of internal study variables (e.g., the amount of money in the participant's "wallet"). |
| `stimuli.js` | The bulk of the actual HTML displayed to the participant. Defines static blocks of HTML (e.g., the consent form, the instructions pages, the demographics survey) as well as blocks that are filled in with experiment variables during the main experiment loop (e.g., the stimuli and questions of the decider trials). |
| `conditions.js` | The logic behind the random assignment of conditions for each participant (e.g., carries out the randomization of the "amount at stake" in each trial). |
| `style.css` | Controls the visual appearance of various experiment elements (e.g., defines the shape and color of the wheel used in Study 3, sets styling for Likert response inputs). |

In addtion, the following auxilliary files may be present:

| Name | Description |
| --- | --- |
| `instructions.html` | A wrapper file around a separate jsPsych "experiment" that simply displays the instructions of the main experiment in a separate browser tab. This was needed to comply with a Prolific policy stating that participants must have access to the instructions when their comprehension thereof is being assessed. |
| `instructions.js` | The logic behind the secondary instructions display described above. Defines the instructions exactly as they are defined in the main experiment. |
| `Macarthur_subjective_SES` | An image of the MacAruthur subjective SES scale, for use in the demographics survey. |
