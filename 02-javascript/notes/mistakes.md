# Mistakes

## Input fields

Wrong

input.textContent

Correct

input.value

Reason

Inputs use value.

Paragraphs use textContent.

## Arrays

Wrong

student.length - 1 == student[i]

Reason

Comparing number to string.

Correct

student[i] === name