# AI Experiments Branch

Welcome to the `ai-experiments` branch! This is your safe space to try out AI-generated R code. Nothing you do here affects `main`, so experiment freely.

## What is "vibecoding"?

Vibecoding is using AI tools (like ChatGPT, Claude, or GitHub Copilot) to help you write code by describing what you want in plain English. You give the AI a prompt, it gives you code, and you try it out.

This is a useful skill, but you need to **check what the AI gives you**. AI-generated code can look right and still be wrong. Practicing here, where you can see whether the output makes biological sense, is a great way to build that judgement.

## How to use this branch

1. Make sure you're on the `ai-experiments` branch (check the branch dropdown on GitHub)
2. Open `run_analysis_SOLUTIONS.R` or create a new `.R` file
3. Use an AI tool to generate some R code (see prompts below)
4. Paste the code into your file and commit it
5. Does it look right? Does the output make biological sense?

## The dataset columns

When writing prompts, it helps to tell the AI exactly what columns are available. After cleaning, the dataset `penguins_clean` has these columns:

| Column | Type | Example values |
|--------|------|---------------|
| `species` | Character | Adelie, Chinstrap, Gentoo |
| `island` | Character | Torgersen, Biscoe, Dream |
| `bill_length_mm` | Numeric | 39.1, 46.5, 50.2 |
| `bill_depth_mm` | Numeric | 18.7, 13.1, 15.2 |
| `flipper_length_mm` | Numeric | 181, 217, 230 |
| `body_mass_g` | Numeric | 3750, 5200, 4800 |
| `sex` | Character | male, female |
| `year` | Integer | 2007, 2008, 2009 |

## Example prompts to try

Here are some prompts you can paste into ChatGPT, Claude, or any AI tool. Copy the code it gives you into an R file on this branch.

### Beginner

> "Write R code using ggplot2 to create a histogram of body_mass_g from a data frame called penguins_clean, coloured by species. Use the colours darkorange for Adelie, purple for Chinstrap, and cyan4 for Gentoo."

> "Write R code to calculate the mean bill_length_mm for each species in a data frame called penguins_clean, using dplyr."

### Intermediate

> "Write R code using ggplot2 to create a scatter plot of bill_length_mm vs bill_depth_mm from penguins_clean, coloured by species, with a linear trend line for each species. Add a title and clean axis labels."

> "Write R code to create a summary table showing the count, mean, and standard deviation of flipper_length_mm for each species and sex combination in penguins_clean."

### Advanced

> "Write R code to perform a one-way ANOVA testing whether body_mass_g differs significantly between species in penguins_clean. Include a post-hoc Tukey test and print the results."

> "Write R code to create a pairs plot (using GGally::ggpairs) of bill_length_mm, bill_depth_mm, flipper_length_mm, and body_mass_g from penguins_clean, coloured by species."

## Checklist of things to try

- [ ] Generate a plot you haven't seen before (histogram, density plot, violin plot)
- [ ] Ask the AI to calculate a summary statistic (mean, median, count by group)
- [ ] Try a statistical test (t-test, ANOVA, correlation)
- [ ] Ask the AI to explain a line of code from `run_analysis_SOLUTIONS.R`
- [ ] Deliberately give the AI a vague prompt and see what happens
- [ ] Try the same prompt in two different AI tools -- do they give the same code?
- [ ] Ask the AI to write code with a bug, then ask it to fix the bug

## Tips

- **Always tell the AI the data frame name** (`penguins_clean`) and the exact column names -- this avoids a lot of errors.
- **Read the code before running it.** Does it use the right column names? Does the logic make sense?
- **If the code doesn't work**, paste the error message back into the AI and ask it to fix it. 
- **Compare AI output to the existing plots** in the analysis. Does the AI's version show the same patterns?
- **Remember:** this branch is yours to experiment with. You can't break anything here that matters.
