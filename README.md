# 24-Hour Nutrition Case Study — Life Stages & Special Diets

A standalone, account-free 24-hour diet-building assessment for HUN1201. Students pick one of seven case scenarios, build a full day of meals from a nutrient database, review a personalized report, and answer 17 questions generated from their own case and food choices.

This is a duplicate of the original "24-Hour Nutrition Case Study" app with:

- An **earth-tone color scheme** (clay/terracotta + ochre/mustard on warm neutrals) in place of the original Valencia red/gold.
- An **Instructions page** shown before the case picker, covering purpose, tasks, success criteria, and how to submit in Canvas.
- **Seven case scenarios** spanning different life stages and dietary patterns: prediabetes/weight loss, muscle gain after illness, a teen athlete, pregnancy on a vegetarian diet, an older adult with heart disease, a new vegan with iron-deficiency anemia, and a picky-eating school-age child.
- A **sixth learning outcome** (Life-Stage & Special Population Nutrition) with two content-knowledge questions per scenario, drawn from the *Energy Balance, Weight Management & Eating Disorders* and *LifeCycle Nutrition* reading modules.

## Files

- `index.html` — the complete standalone app.

## Publish with GitHub Pages

If GitHub Pages is already enabled for this repository (see the root `README.md`), this app is automatically served at:

`https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/nutrition-case-study/`

No separate Pages setup is needed — GitHub Pages serves the whole repository, including subfolders.

## Embed in Canvas

Use the same iframe pattern as `canvas-embed-code.txt` in the repository root, pointing the `src` at the URL above instead.

## Customize

- Case data (including special considerations, diet pattern, and life-stage DRI overrides) lives in the `SCENARIOS` array and `driTargetsFor()` function near the top of the embedded script in `index.html`.
- Scenario-specific Learning Outcome 6 questions live in the `lo6Pool` object inside `generateQuestions()`.
- After changing case or question data, increase `QUESTION_SET_VERSION` so previously saved student sessions don't conflict with the new structure.
