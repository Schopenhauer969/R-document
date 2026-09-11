# 📊 R Programming — Beginner to Advanced

> A complete R programming guide from **Beginner → Intermediate → Advanced**, with practical examples, full code, and explanations in **English + Khmer**.

![R](https://img.shields.io/badge/R-Programming-276DC3?style=for-the-badge\&logo=r\&logoColor=white)
![Level](https://img.shields.io/badge/Level-Beginner%20→%20Advanced-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

---

## 📚 Table of Contents

* [1. What is R?](#1-what-is-r)
* [2. Installing R](#2-installing-r)
* [3. Your First R Program](#3-your-first-r-program)
* [4. Comments](#4-comments)
* [5. Variables](#5-variables)
* [6. Data Types](#6-data-types)
* [7. Operators](#7-operators)
* [8. Strings](#8-strings)
* [9. Input and Output](#9-input-and-output)
* [10. Conditional Statements](#10-conditional-statements)
* [11. Loops](#11-loops)
* [12. Functions](#12-functions)
* [13. Vectors](#13-vectors)
* [14. Lists](#14-lists)
* [15. Matrices](#15-matrices)
* [16. Arrays](#16-arrays)
* [17. Factors](#17-factors)
* [18. Data Frames](#18-data-frames)
* [19. Missing Values](#19-missing-values)
* [20. Dates and Times](#20-dates-and-times)
* [21. Apply Family](#21-apply-family)
* [22. File Handling](#22-file-handling)
* [23. Packages](#23-packages)
* [24. Data Manipulation with dplyr](#24-data-manipulation-with-dplyr)
* [25. Data Visualization with ggplot2](#25-data-visualization-with-ggplot2)
* [26. Statistics](#26-statistics)
* [27. Probability](#27-probability)
* [28. Linear Regression](#28-linear-regression)
* [29. Multiple Regression](#29-multiple-regression)
* [30. Classification](#30-classification)
* [31. Correlation](#31-correlation)
* [32. SQL and Databases](#32-sql-and-databases)
* [33. Web APIs](#33-web-apis)
* [34. JSON](#34-json)
* [35. Object-Oriented Programming](#35-object-oriented-programming)
* [36. Error Handling](#36-error-handling)
* [37. Functional Programming](#37-functional-programming)
* [38. Environments](#38-environments)
* [39. Advanced Data Manipulation](#39-advanced-data-manipulation)
* [40. R Markdown](#40-r-markdown)
* [41. Shiny](#41-shiny)
* [42. Testing](#42-testing)
* [43. Project Structure](#43-project-structure)
* [44. Best Practices](#44-best-practices)
* [45. Complete Beginner Project](#45-complete-beginner-project)
* [46. Complete Intermediate Project](#46-complete-intermediate-project)
* [47. Complete Advanced Project](#47-complete-advanced-project)
* [48. Learning Roadmap](#48-learning-roadmap)

---

# 1. What is R?

## English

**R** is a programming language and environment designed mainly for:

* Data analysis
* Statistics
* Data visualization
* Machine learning
* Scientific computing
* Research
* Reporting

R is especially popular in **data science, statistics, finance, biology, research, and analytics**.

## ភាសាខ្មែរ

**R** គឺជាភាសាកម្មវិធីដែលត្រូវបានបង្កើតឡើងសម្រាប់៖

* ការវិភាគទិន្នន័យ
* ស្ថិតិ
* ការបង្ហាញទិន្នន័យជាក្រាហ្វ
* Machine Learning
* Scientific Computing
* Research
* Data Analytics

---

# 2. Installing R

Download R from:

https://cran.r-project.org/

You can also use **RStudio**, which provides a convenient development environment for R.

Basic installation check:

```r
R.version.string
```

Example output:

```text
[1] "R version 4.x.x ..."
```

## Khmer

ដើម្បីសរសេរ R ឲ្យងាយស្រួល អ្នកអាចប្រើ **RStudio** ជាមួយ R។

---

# 3. Your First R Program

Create a file:

```text
hello.R
```

Add:

```r
print("Hello, World!")
```

Run it.

Output:

```text
[1] "Hello, World!"
```

You can also write:

```r
message("Hello, R!")
```

## Khmer

`print()` ប្រើសម្រាប់បង្ហាញតម្លៃទៅកាន់ Console។

---

# 4. Comments

Comments are ignored by R.

```r
# This is a comment

print("Hello")
```

Multiple lines:

```r
# Calculate total price
# Add tax
# Display result

price <- 100
tax <- 10

total <- price + tax

print(total)
```

## Khmer

Comment ចាប់ផ្តើមដោយ `#`។

វាមិនត្រូវបាន Execute ទេ ហើយប្រើសម្រាប់ពន្យល់ Code។

---

# 5. Variables

R uses `<-` commonly for assignment.

```r
name <- "Dara"
age <- 20
height <- 1.75
is_student <- TRUE

print(name)
print(age)
print(height)
print(is_student)
```

You can also use:

```r
x = 10
```

But `<-` is the conventional R style.

## Variable naming

Good:

```r
first_name <- "Dara"
student_age <- 20
total_price <- 100
```

Avoid:

```r
1name <- "Dara"
```

## Khmer

Variable គឺជាឈ្មោះដែលយើងប្រើដើម្បីរក្សាទុកទិន្នន័យ។

ឧទាហរណ៍៖

```r
name <- "Dara"
```

មានន័យថា Variable `name` មានតម្លៃ `"Dara"`។

---

# 6. Data Types

Common R data types:

* Character
* Numeric
* Integer
* Logical
* Complex

## Character

```r
name <- "Dara"

print(name)
class(name)
```

## Numeric

```r
price <- 99.99

print(price)
class(price)
```

## Integer

```r
age <- 20L

print(age)
class(age)
```

## Logical

```r
is_student <- TRUE

print(is_student)
class(is_student)
```

## Complex

```r
number <- 3 + 2i

print(number)
class(number)
```

## Khmer

Data Type ប្រាប់យើងថា data មួយមានប្រភេទអ្វី។

ឧទាហរណ៍៖

```r
name <- "Dara"
```

ជា `character`។

```r
age <- 20L
```

ជា `integer`។

---

# 7. Operators

## Arithmetic Operators

```r
a <- 10
b <- 3

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a ^ b)
print(a %% b)
print(a %/% b)
```

Meaning:

| Operator | Meaning          |
| -------- | ---------------- |
| `+`      | Addition         |
| `-`      | Subtraction      |
| `*`      | Multiplication   |
| `/`      | Division         |
| `^`      | Power            |
| `%%`     | Modulo           |
| `%/%`    | Integer division |

## Comparison Operators

```r
a <- 10
b <- 20

print(a == b)
print(a != b)
print(a > b)
print(a < b)
print(a >= b)
print(a <= b)
```

## Logical Operators

```r
x <- TRUE
y <- FALSE

print(x & y)
print(x | y)
print(!x)
```

## Khmer

Operators គឺជា symbols ដែលប្រើសម្រាប់គណនា និងប្រៀបធៀបតម្លៃ។

---

# 8. Strings

```r
first_name <- "Dara"
last_name <- "Sok"

full_name <- paste(first_name, last_name)

print(full_name)
```

Using `paste0()`:

```r
first_name <- "Dara"
last_name <- "Sok"

full_name <- paste0(first_name, " ", last_name)

print(full_name)
```

String length:

```r
text <- "Hello R"

print(nchar(text))
```

Convert case:

```r
text <- "Hello R Programming"

print(toupper(text))
print(tolower(text))
```

Substring:

```r
text <- "Programming"

print(substr(text, 1, 4))
```

## Khmer

String គឺជា Text។

ឧទាហរណ៍៖

```r
name <- "Dara"
```

---

# 9. Input and Output

## Print

```r
name <- "Dara"

print(name)
```

## Read input

```r
name <- readline("Enter your name: ")

cat("Hello,", name, "\n")
```

## Numeric input

`readline()` returns character data, so convert it:

```r
age <- as.numeric(readline("Enter your age: "))

cat("Your age is:", age, "\n")
```

## Khmer

`readline()` ប្រើសម្រាប់ទទួល Input ពី User។

---

# 10. Conditional Statements

## if

```r
age <- 20

if (age >= 18) {
  print("Adult")
}
```

## if else

```r
age <- 16

if (age >= 18) {
  print("Adult")
} else {
  print("Minor")
}
```

## else if

```r
score <- 85

if (score >= 90) {
  print("A")
} else if (score >= 80) {
  print("B")
} else if (score >= 70) {
  print("C")
} else {
  print("F")
}
```

## Multiple conditions

```r
age <- 20
has_id <- TRUE

if (age >= 18 && has_id) {
  print("Allowed")
} else {
  print("Not allowed")
}
```

## Khmer

Conditional Statement ប្រើសម្រាប់សម្រេចថា Code ត្រូវធ្វើអ្វីនៅពេល Condition ពិត ឬមិនពិត។

---

# 11. Loops

## for loop

```r
for (i in 1:5) {
  print(i)
}
```

## Loop through vector

```r
names <- c("Dara", "Sok", "Chan")

for (name in names) {
  print(name)
}
```

## while loop

```r
counter <- 1

while (counter <= 5) {
  print(counter)
  counter <- counter + 1
}
```

## break

```r
for (i in 1:10) {
  if (i == 5) {
    break
  }

  print(i)
}
```

## next

```r
for (i in 1:5) {
  if (i == 3) {
    next
  }

  print(i)
}
```

## Khmer

Loop ប្រើសម្រាប់ធ្វើការងារដដែលៗច្រើនដង។

---

# 12. Functions

Basic function:

```r
greet <- function(name) {
  message <- paste("Hello", name)
  return(message)
}

result <- greet("Dara")

print(result)
```

Function with multiple parameters:

```r
add <- function(a, b) {
  return(a + b)
}

result <- add(10, 20)

print(result)
```

Default parameter:

```r
greet <- function(name = "Guest") {
  paste("Hello", name)
}

print(greet())
print(greet("Dara"))
```

Function with condition:

```r
calculate_grade <- function(score) {
  if (score >= 90) {
    return("A")
  } else if (score >= 80) {
    return("B")
  } else if (score >= 70) {
    return("C")
  } else {
    return("F")
  }
}

print(calculate_grade(85))
```

## Khmer

Function គឺជា Block នៃ Code ដែលអាចយកមកប្រើឡើងវិញ។

---

# 13. Vectors

A vector stores multiple values of the same basic type.

```r
numbers <- c(10, 20, 30, 40, 50)

print(numbers)
```

Access elements:

```r
numbers <- c(10, 20, 30, 40, 50)

print(numbers[1])
print(numbers[3])
print(numbers[1:3])
```

Vector operations:

```r
numbers <- c(10, 20, 30, 40, 50)

print(numbers + 10)
print(numbers * 2)
print(sum(numbers))
print(mean(numbers))
print(max(numbers))
print(min(numbers))
```

Named vector:

```r
scores <- c(
  Dara = 90,
  Sok = 85,
  Chan = 95
)

print(scores)
print(scores["Dara"])
```

## Khmer

Vector គឺជា Collection នៃតម្លៃជាច្រើន ដែលជាទូទៅមាន Type ដូចគ្នា។

---

# 14. Lists

A list can contain different types of data.

```r
person <- list(
  name = "Dara",
  age = 20,
  scores = c(80, 90, 85),
  active = TRUE
)

print(person)
```

Access values:

```r
print(person$name)
print(person$age)
print(person$scores)
```

Alternative:

```r
print(person[["name"]])
```

Modify:

```r
person$age <- 21

print(person$age)
```

## Khmer

List អាចរក្សាទុក Data ប្រភេទផ្សេងៗគ្នា នៅក្នុង Object តែមួយ។

---

# 15. Matrices

A matrix is a two-dimensional structure.

```r
matrix_data <- matrix(
  1:6,
  nrow = 2,
  ncol = 3
)

print(matrix_data)
```

Create by rows:

```r
matrix_data <- matrix(
  1:6,
  nrow = 2,
  byrow = TRUE
)

print(matrix_data)
```

Access:

```r
print(matrix_data[1, 2])
```

Matrix multiplication:

```r
A <- matrix(c(1, 2, 3, 4), nrow = 2)
B <- matrix(c(5, 6, 7, 8), nrow = 2)

print(A %*% B)
```

---

# 16. Arrays

Arrays can have more than two dimensions.

```r
data <- array(
  1:12,
  dim = c(2, 3, 2)
)

print(data)
```

Access:

```r
print(data[1, 2, 1])
```

## Khmer

Array គឺជា Data Structure ដែលអាចមានច្រើនជាង 2 dimensions។

---

# 17. Factors

Factors are useful for categorical data.

```r
gender <- factor(
  c("Male", "Female", "Male", "Female")
)

print(gender)
print(levels(gender))
```

Ordered factor:

```r
size <- factor(
  c("Small", "Large", "Medium"),
  levels = c("Small", "Medium", "Large"),
  ordered = TRUE
)

print(size)
print(size[1] < size[2])
```

## Khmer

Factor ប្រើសម្រាប់ Data ដែលមាន Category ដូចជា៖

* Male / Female
* Small / Medium / Large
* Beginner / Intermediate / Advanced

---

# 18. Data Frames

A data frame is one of the most important R structures for data analysis.

```r
students <- data.frame(
  id = c(1, 2, 3, 4),
  name = c("Dara", "Sok", "Chan", "Vanna"),
  age = c(20, 21, 19, 22),
  score = c(85, 90, 78, 95)
)

print(students)
```

Access columns:

```r
print(students$name)
print(students$score)
```

Access rows:

```r
print(students[1, ])
```

Access specific cell:

```r
print(students[1, 2])
```

Filter:

```r
result <- students[students$score >= 85, ]

print(result)
```

Add column:

```r
students$passed <- students$score >= 50

print(students)
```

Sort:

```r
students_sorted <- students[
  order(students$score, decreasing = TRUE),
]

print(students_sorted)
```

## Khmer

Data Frame គឺជា Structure សំខាន់បំផុតមួយសម្រាប់ Data Analysis ក្នុង R។

វាមានរូបរាងដូចជា Table៖

| id | name | age | score |
| -: | ---- | --: | ----: |
|  1 | Dara |  20 |    85 |
|  2 | Sok  |  21 |    90 |

---

# 19. Missing Values

R represents missing data with `NA`.

```r
scores <- c(80, 90, NA, 70, 85)

print(scores)
```

Check missing values:

```r
print(is.na(scores))
```

Count missing values:

```r
print(sum(is.na(scores)))
```

Remove missing values:

```r
clean_scores <- na.omit(scores)

print(clean_scores)
```

Calculate mean while ignoring missing values:

```r
scores <- c(80, 90, NA, 70, 85)

print(mean(scores, na.rm = TRUE))
```

## Khmer

`NA` មានន័យថា Data មិនមានតម្លៃ ឬ Missing។

---

# 20. Dates and Times

Current date:

```r
today <- Sys.Date()

print(today)
```

Current date and time:

```r
now <- Sys.time()

print(now)
```

Create a date:

```r
birthday <- as.Date("2000-05-15")

print(birthday)
```

Date calculation:

```r
date <- as.Date("2026-01-01")

print(date + 30)
```

Date difference:

```r
start <- as.Date("2026-01-01")
end <- as.Date("2026-01-31")

difference <- end - start

print(difference)
```

---

# 21. Apply Family

The apply family is important for writing cleaner R code.

## lapply

```r
numbers <- list(
  a = 1:5,
  b = 6:10,
  c = 11:15
)

result <- lapply(numbers, sum)

print(result)
```

## sapply

```r
numbers <- list(
  a = 1:5,
  b = 6:10,
  c = 11:15
)

result <- sapply(numbers, sum)

print(result)
```

## apply

```r
matrix_data <- matrix(1:9, nrow = 3)

row_sums <- apply(matrix_data, 1, sum)
column_sums <- apply(matrix_data, 2, sum)

print(row_sums)
print(column_sums)
```

## vapply

```r
numbers <- list(
  a = 1:5,
  b = 6:10
)

result <- vapply(
  numbers,
  sum,
  numeric(1)
)

print(result)
```

## Khmer

Apply Family ជួយឲ្យយើងធ្វើការជាមួយ Collection/Data ដោយកាត់បន្ថយ `for` loop។

---

# 22. File Handling

## Write text

```r
text <- "Hello from R!"

writeLines(
  text,
  "example.txt"
)
```

## Read text

```r
content <- readLines("example.txt")

print(content)
```

## Write CSV

```r
students <- data.frame(
  name = c("Dara", "Sok", "Chan"),
  score = c(80, 90, 85)
)

write.csv(
  students,
  "students.csv",
  row.names = FALSE
)
```

## Read CSV

```r
students <- read.csv("students.csv")

print(students)
```

## Khmer

R អាចអាន និងសរសេរ File ដូចជា៖

* `.txt`
* `.csv`
* `.rds`
* Excel និងប្រភេទផ្សេងៗតាម Package។

---

# 23. Packages

Packages extend R's functionality.

Install a package:

```r
install.packages("dplyr")
```

Load a package:

```r
library(dplyr)
```

Check installed packages:

```r
installed.packages()
```

Remove a package:

```r
remove.packages("dplyr")
```

## Khmer

Package គឺជា Library ដែលបន្ថែមមុខងារថ្មីៗទៅ R។

---

# 24. Data Manipulation with dplyr

Install:

```r
install.packages("dplyr")
```

Load:

```r
library(dplyr)
```

Create data:

```r
students <- data.frame(
  name = c("Dara", "Sok", "Chan", "Vanna"),
  age = c(20, 21, 19, 22),
  score = c(85, 90, 78, 95)
)
```

## select

```r
result <- students %>%
  select(name, score)

print(result)
```

## filter

```r
result <- students %>%
  filter(score >= 85)

print(result)
```

## mutate

```r
result <- students %>%
  mutate(
    passed = score >= 50
  )

print(result)
```

## arrange

```r
result <- students %>%
  arrange(desc(score))

print(result)
```

## summarise

```r
result <- students %>%
  summarise(
    average_score = mean(score),
    highest_score = max(score),
    lowest_score = min(score)
  )

print(result)
```

## Full example

```r
library(dplyr)

students <- data.frame(
  name = c("Dara", "Sok", "Chan", "Vanna"),
  class = c("A", "A", "B", "B"),
  score = c(85, 90, 78, 95)
)

result <- students %>%
  filter(score >= 80) %>%
  mutate(
    grade = case_when(
      score >= 90 ~ "A",
      score >= 80 ~ "B",
      score >= 70 ~ "C",
      TRUE ~ "F"
    )
  ) %>%
  arrange(desc(score))

print(result)
```

## Khmer

`dplyr` គឺជា Package ដ៏ពេញនិយមសម្រាប់ Data Manipulation។

Functions សំខាន់ៗ៖

* `select()`
* `filter()`
* `mutate()`
* `arrange()`
* `summarise()`
* `group_by()`

---

# 25. Data Visualization with ggplot2

Install:

```r
install.packages("ggplot2")
```

Load:

```r
library(ggplot2)
```

Create data:

```r
students <- data.frame(
  name = c("Dara", "Sok", "Chan", "Vanna"),
  score = c(85, 90, 78, 95)
)
```

## Bar chart

```r
library(ggplot2)

ggplot(
  students,
  aes(x = name, y = score)
) +
  geom_col() +
  labs(
    title = "Student Scores",
    x = "Student",
    y = "Score"
)
```

## Scatter plot

```r
data <- data.frame(
  hours = c(1, 2, 3, 4, 5, 6),
  score = c(50, 55, 65, 70, 80, 90)
)

ggplot(
  data,
  aes(x = hours, y = score)
) +
  geom_point() +
  labs(
    title = "Study Hours vs Score",
    x = "Study Hours",
    y = "Score"
  )
```

## Line chart

```r
data <- data.frame(
  day = 1:7,
  sales = c(10, 15, 13, 20, 25, 22, 30)
)

ggplot(
  data,
  aes(x = day, y = sales)
) +
  geom_line() +
  geom_point() +
  labs(
    title = "Weekly Sales",
    x = "Day",
    y = "Sales"
  )
```

## Histogram

```r
data <- data.frame(
  score = c(
    50, 55, 60, 62, 65,
    68, 70, 72, 75, 78,
    80, 82, 85, 88, 90,
    92, 95, 98
  )
)

ggplot(
  data,
  aes(x = score)
) +
  geom_histogram(
    bins = 6
  ) +
  labs(
    title = "Score Distribution",
    x = "Score",
    y = "Frequency"
  )
```

## Khmer

`ggplot2` ប្រើសម្រាប់បង្កើត Visualization ដែលមានគុណភាពខ្ពស់។

---

# 26. Statistics

## Mean

```r
scores <- c(70, 80, 90, 100)

print(mean(scores))
```

## Median

```r
scores <- c(10, 20, 30, 40, 100)

print(median(scores))
```

## Standard deviation

```r
scores <- c(70, 80, 90, 100)

print(sd(scores))
```

## Variance

```r
scores <- c(70, 80, 90, 100)

print(var(scores))
```

## Summary

```r
scores <- c(70, 80, 90, 100)

print(summary(scores))
```

## Khmer

Statistics ប្រើសម្រាប់ស្វែងយល់ពី Distribution និង Characteristics របស់ Data។

---

# 27. Probability

Generate random numbers:

```r
set.seed(123)

numbers <- runif(
  10,
  min = 0,
  max = 1
)

print(numbers)
```

Random integers:

```r
set.seed(123)

numbers <- sample(
  1:100,
  10
)

print(numbers)
```

Random sampling:

```r
students <- c(
  "Dara",
  "Sok",
  "Chan",
  "Vanna",
  "Kanha"
)

set.seed(123)

selected <- sample(
  students,
  2
)

print(selected)
```

Normal distribution:

```r
set.seed(123)

values <- rnorm(
  1000,
  mean = 100,
  sd = 15
)

print(mean(values))
```

---

# 28. Linear Regression

Create data:

```r
data <- data.frame(
  hours = c(1, 2, 3, 4, 5, 6),
  score = c(50, 55, 65, 70, 80, 90)
)
```

Train model:

```r
model <- lm(
  score ~ hours,
  data = data
)

print(model)
```

View results:

```r
summary(model)
```

Predict:

```r
new_data <- data.frame(
  hours = c(7, 8)
)

predictions <- predict(
  model,
  newdata = new_data
)

print(predictions)
```

Plot:

```r
plot(
  data$hours,
  data$score,
  main = "Study Hours vs Score",
  xlab = "Study Hours",
  ylab = "Score"
)

abline(
  model
)
```

## Khmer

Linear Regression ប្រើសម្រាប់ស្វែងរកទំនាក់ទំនងរវាង Variables និងធ្វើ Prediction។

ឧទាហរណ៍៖

> Study Hours → Exam Score

---

# 29. Multiple Regression

```r
data <- data.frame(
  hours = c(1, 2, 3, 4, 5, 6, 7, 8),
  attendance = c(60, 65, 70, 75, 80, 85, 90, 95),
  score = c(50, 55, 60, 68, 75, 80, 88, 94)
)

model <- lm(
  score ~ hours + attendance,
  data = data
)

summary(model)
```

Prediction:

```r
new_student <- data.frame(
  hours = 6,
  attendance = 85
)

prediction <- predict(
  model,
  newdata = new_student
)

print(prediction)
```

---

# 30. Classification

A simple logistic regression example:

```r
students <- data.frame(
  hours = c(1, 2, 3, 4, 5, 6, 7, 8),
  passed = c(
    0, 0, 0, 0,
    1, 1, 1, 1
  )
)

model <- glm(
  passed ~ hours,
  data = students,
  family = binomial()
)

summary(model)
```

Prediction:

```r
new_students <- data.frame(
  hours = c(2.5, 5.5, 7.5)
)

probabilities <- predict(
  model,
  newdata = new_students,
  type = "response"
)

print(probabilities)
```

Convert probability to class:

```r
predicted_class <- ifelse(
  probabilities >= 0.5,
  1,
  0
)

print(predicted_class)
```

## Khmer

Classification គឺការទស្សន៍ទាយ Category/Class។

ឧទាហរណ៍៖

```text
0 = Fail
1 = Pass
```

---

# 31. Correlation

```r
hours <- c(1, 2, 3, 4, 5, 6)
scores <- c(50, 55, 65, 70, 80, 90)

correlation <- cor(
  hours,
  scores
)

print(correlation)
```

Correlation matrix:

```r
data <- data.frame(
  hours = c(1, 2, 3, 4, 5),
  score = c(50, 60, 70, 80, 90),
  attendance = c(60, 65, 75, 85, 95)
)

print(cor(data))
```

## Khmer

Correlation ប្រើសម្រាប់វាស់ទំនាក់ទំនងរវាង Variables។

---

# 32. SQL and Databases

Install DBI and RSQLite:

```r
install.packages("DBI")
install.packages("RSQLite")
```

Connect to database:

```r
library(DBI)
library(RSQLite)

connection <- dbConnect(
  SQLite(),
  "students.db"
)
```

Create table:

```r
students <- data.frame(
  id = 1:3,
  name = c("Dara", "Sok", "Chan"),
  score = c(85, 90, 78)
)

dbWriteTable(
  connection,
  "students",
  students,
  overwrite = TRUE
)
```

Query:

```r
result <- dbGetQuery(
  connection,
  "SELECT * FROM students"
)

print(result)
```

Filter with SQL:

```r
result <- dbGetQuery(
  connection,
  "SELECT * FROM students WHERE score >= 80"
)

print(result)
```

Close connection:

```r
dbDisconnect(connection)
```

## Khmer

R អាចភ្ជាប់ជាមួយ Database ដូចជា SQLite, PostgreSQL និង MySQL តាមរយៈ Packages។

---

# 33. Web APIs

Install `httr2`:

```r
install.packages("httr2")
```

Example API request:

```r
library(httr2)

request <- request(
  "https://httpbin.org/get"
)

response <- req_perform(request)

print(resp_status(response))
```

Read response:

```r
body <- resp_body_json(response)

print(body)
```

## Khmer

API អនុញ្ញាតឲ្យ R ទាក់ទងជាមួយ Web Services។

---

# 34. JSON

Install `jsonlite`:

```r
install.packages("jsonlite")
```

Convert R object to JSON:

```r
library(jsonlite)

person <- list(
  name = "Dara",
  age = 20,
  active = TRUE
)

json_data <- toJSON(
  person,
  auto_unbox = TRUE,
  pretty = TRUE
)

cat(json_data)
```

JSON to R:

```r
json_text <- '{
  "name": "Dara",
  "age": 20,
  "active": true
}'

person <- fromJSON(json_text)

print(person)
```

---

# 35. Object-Oriented Programming

R has several object-oriented systems.

One simple approach is S3.

## Create an S3 object

```r
create_person <- function(name, age) {
  person <- list(
    name = name,
    age = age
  )

  class(person) <- "Person"

  return(person)
}
```

Create object:

```r
person <- create_person(
  "Dara",
  20
)

print(person)
```

Create method:

```r
print.Person <- function(x, ...) {
  cat(
    "Name:",
    x$name,
    "\n"
  )

  cat(
    "Age:",
    x$age,
    "\n"
  )
}
```

Full example:

```r
create_person <- function(name, age) {
  person <- list(
    name = name,
    age = age
  )

  class(person) <- "Person"

  person
}

print.Person <- function(x, ...) {
  cat("Name:", x$name, "\n")
  cat("Age:", x$age, "\n")
}

person <- create_person(
  "Dara",
  20
)

print(person)
```

## Khmer

S3 គឺជា Object-Oriented System មួយរបស់ R ដែលមានភាពសាមញ្ញ និងប្រើប្រាស់ទូលំទូលាយ។

---

# 36. Error Handling

## tryCatch

```r
safe_divide <- function(a, b) {
  tryCatch(
    {
      if (b == 0) {
        stop("Cannot divide by zero")
      }

      a / b
    },
    error = function(e) {
      message(
        "Error: ",
        e$message
      )

      NA_real_
    }
  )
}

print(safe_divide(10, 2))
print(safe_divide(10, 0))
```

## Warning

```r
check_age <- function(age) {
  if (age < 0) {
    warning("Age cannot be negative")
  }

  age
}

print(check_age(-5))
```

## Khmer

Error Handling ជួយឲ្យ Program មិន Crash ងាយៗ និងអាចគ្រប់គ្រង Error បានល្អ។

---

# 37. Functional Programming

R supports functions as first-class objects.

Function stored in variable:

```r
square <- function(x) {
  x * x
}

print(square(5))
```

Function passed to another function:

```r
numbers <- 1:5

result <- sapply(
  numbers,
  square
)

print(result)
```

Anonymous function:

```r
numbers <- 1:5

result <- sapply(
  numbers,
  function(x) {
    x * 2
  }
)

print(result)
```

---

# 38. Environments

Create environment:

```r
env <- new.env()

env$name <- "Dara"
env$age <- 20

print(env$name)
print(env$age)
```

List environment contents:

```r
print(ls(env))
```

Check variable:

```r
print(exists("name", envir = env))
```

## Khmer

Environment គឺជា Data Structure ដែលរក្សាទុក Key-Value bindings និងមានសារៈសំខាន់សម្រាប់ Scope និង Advanced R Programming។

---

# 39. Advanced Data Manipulation

## group_by

```r
library(dplyr)

students <- data.frame(
  class = c("A", "A", "B", "B"),
  score = c(80, 90, 70, 100)
)

result <- students %>%
  group_by(class) %>%
  summarise(
    average = mean(score),
    maximum = max(score),
    minimum = min(score)
  )

print(result)
```

## Multiple transformations

```r
library(dplyr)

students <- data.frame(
  name = c(
    "Dara",
    "Sok",
    "Chan",
    "Vanna"
  ),
  class = c(
    "A",
    "A",
    "B",
    "B"
  ),
  score = c(
    85,
    90,
    78,
    95
  )
)

result <- students %>%
  mutate(
    passed = score >= 50
  ) %>%
  group_by(class) %>%
  summarise(
    students = n(),
    average_score = mean(score),
    highest_score = max(score)
  ) %>%
  arrange(desc(average_score))

print(result)
```

---

# 40. R Markdown

R Markdown allows you to combine:

* R code
* Text
* Tables
* Charts
* Analysis
* Reports

A basic `.Rmd` file:

````markdown
---
title: "Student Report"
author: "Dara"
output: html_document
---

# Introduction

This report analyzes student scores.

```{r}
students <- data.frame(
  name = c("Dara", "Sok", "Chan"),
  score = c(85, 90, 78)
)

students
```

## Average Score

```{r}
mean(students$score)
```
````

## Khmer

R Markdown អនុញ្ញាតឲ្យយើងសរសេរ Documentation និង Data Analysis នៅក្នុង File តែមួយ។

---

# 41. Shiny

Shiny is used to build interactive web applications with R.

Install:

```r
install.packages("shiny")
```

Create `app.R`:

```r
library(shiny)

ui <- fluidPage(
  titlePanel("My First Shiny App"),

  sidebarLayout(
    sidebarPanel(
      sliderInput(
        "number",
        "Choose a number:",
        min = 1,
        max = 100,
        value = 50
      )
    ),

    mainPanel(
      textOutput("result")
    )
  )
)

server <- function(input, output, session) {
  output$result <- renderText({
    paste(
      "You selected:",
      input$number
    )
  })
}

shinyApp(
  ui = ui,
  server = server
)
```

Run:

```r
shiny::runApp()
```

## Khmer

Shiny អនុញ្ញាតឲ្យយើងបង្កើត Web Application ដោយប្រើ R។

---

# 42. Testing

For serious projects, automated tests are important.

Install testthat:

```r
install.packages("testthat")
```

Example function:

```r
add <- function(a, b) {
  a + b
}
```

Test:

```r
library(testthat)

test_that(
  "add returns correct result",
  {
    expect_equal(
      add(2, 3),
      5
    )
  }
)
```

Another test:

```r
test_that(
  "add handles negative numbers",
  {
    expect_equal(
      add(-2, 5),
      3
    )
  }
)
```

## Khmer

Testing ជួយធានាថា Code របស់យើងដំណើរការត្រឹមត្រូវ និងជួយរក Bug មុនពេល Deploy។

---

# 43. Project Structure

A professional R project can use this structure:

```text
my-r-project/
│
├── README.md
├── DESCRIPTION
├── LICENSE
├── .gitignore
│
├── R/
│   ├── functions.R
│   └── helpers.R
│
├── data/
│   ├── raw/
│   └── processed/
│
├── tests/
│   └── testthat/
│       └── test-functions.R
│
├── scripts/
│   └── analysis.R
│
├── reports/
│   └── report.Rmd
│
└── outputs/
    ├── figures/
    └── tables/
```

## Khmer

Project ដែលមានទំហំធំគួររៀបចំ Folder ឲ្យច្បាស់ ដើម្បីងាយស្រួល៖

* Maintain
* Test
* Collaborate
* Deploy
* Document

---

# 44. Best Practices

## 1. Use meaningful names

Good:

```r
student_average_score <- 85
```

Bad:

```r
x <- 85
```

## 2. Use functions

Instead of:

```r
a <- 10
b <- 20
c <- a + b
```

Prefer reusable logic:

```r
add <- function(a, b) {
  a + b
}

result <- add(10, 20)
```

## 3. Avoid unnecessary global variables

Prefer:

```r
calculate_total <- function(price, tax) {
  price + tax
}
```

Instead of relying on global variables.

## 4. Comment the reason, not obvious code

Bad:

```r
# Add 1 to counter
counter <- counter + 1
```

Better:

```r
# Move to the next page
counter <- counter + 1
```

## 5. Keep code readable

Good:

```r
result <- students %>%
  filter(score >= 80) %>%
  arrange(desc(score))
```

Avoid unnecessarily complicated one-line code.

---

# 45. Complete Beginner Project

## Student Grade Calculator

Create:

```text
student_grade.R
```

Full code:

```r
calculate_grade <- function(score) {
  if (score >= 90) {
    "A"
  } else if (score >= 80) {
    "B"
  } else if (score >= 70) {
    "C"
  } else if (score >= 60) {
    "D"
  } else {
    "F"
  }
}

name <- readline("Enter student name: ")

score <- as.numeric(
  readline("Enter score: ")
)

if (is.na(score) || score < 0 || score > 100) {
  stop(
    "Score must be a number between 0 and 100."
  )
}

grade <- calculate_grade(score)

cat(
  "\nStudent:",
  name,
  "\n"
)

cat(
  "Score:",
  score,
  "\n"
)

cat(
  "Grade:",
  grade,
  "\n"
)
```

### Example

```text
Enter student name: Dara
Enter score: 85

Student: Dara
Score: 85
Grade: B
```

---

# 46. Complete Intermediate Project

## Student Data Analysis

Install packages:

```r
install.packages("dplyr")
install.packages("ggplot2")
```

Full code:

```r
library(dplyr)
library(ggplot2)

students <- data.frame(
  name = c(
    "Dara",
    "Sok",
    "Chan",
    "Vanna",
    "Kanha",
    "Bora"
  ),
  class = c(
    "A",
    "A",
    "B",
    "B",
    "A",
    "B"
  ),
  score = c(
    85,
    90,
    78,
    95,
    88,
    72
  )
)

students <- students %>%
  mutate(
    grade = case_when(
      score >= 90 ~ "A",
      score >= 80 ~ "B",
      score >= 70 ~ "C",
      score >= 60 ~ "D",
      TRUE ~ "F"
    ),
    passed = score >= 50
  )

print(students)

summary_data <- students %>%
  group_by(class) %>%
  summarise(
    students = n(),
    average_score = mean(score),
    highest_score = max(score),
    lowest_score = min(score)
  )

print(summary_data)

ggplot(
  students,
  aes(
    x = name,
    y = score
  )
) +
  geom_col() +
  labs(
    title = "Student Scores",
    x = "Student",
    y = "Score"
  )
```

---

# 47. Complete Advanced Project

## Student Prediction Project

This project demonstrates:

1. Data creation
2. Data visualization
3. Model training
4. Prediction
5. Evaluation

Full code:

```r
library(ggplot2)

set.seed(123)

students <- data.frame(
  study_hours = c(
    1, 2, 2, 3, 3,
    4, 4, 5, 5, 6,
    6, 7, 7, 8, 8
  ),
  attendance = c(
    60, 65, 68, 70, 72,
    75, 78, 80, 82, 85,
    87, 90, 92, 95, 98
  ),
  score = c(
    45, 50, 53, 58, 62,
    68, 70, 75, 78, 82,
    85, 88, 91, 95, 98
  )
)

# -----------------------------
# 1. Explore the data
# -----------------------------

print(students)
print(summary(students))

# -----------------------------
# 2. Visualize the data
# -----------------------------

ggplot(
  students,
  aes(
    x = study_hours,
    y = score
  )
) +
  geom_point() +
  labs(
    title = "Study Hours vs Score",
    x = "Study Hours",
    y = "Score"
  )

# -----------------------------
# 3. Train model
# -----------------------------

model <- lm(
  score ~ study_hours + attendance,
  data = students
)

print(summary(model))

# -----------------------------
# 4. Make prediction
# -----------------------------

new_student <- data.frame(
  study_hours = 6,
  attendance = 90
)

prediction <- predict(
  model,
  newdata = new_student
)

cat(
  "Predicted score:",
  prediction,
  "\n"
)

# -----------------------------
# 5. Model predictions
# -----------------------------

students$predicted_score <- predict(
  model,
  newdata = students
)

print(students)

# -----------------------------
# 6. Calculate RMSE
# -----------------------------

rmse <- sqrt(
  mean(
    (students$score -
       students$predicted_score)^2
  )
)

cat(
  "RMSE:",
  rmse,
  "\n"
)
```

## Khmer

Project នេះបង្ហាញ Workflow ដែលប្រើក្នុង Data Science ពិតៗ៖

```text
Data
 ↓
Exploration
 ↓
Visualization
 ↓
Model
 ↓
Prediction
 ↓
Evaluation
```

---

# 48. Learning Roadmap

## 🟢 Level 1 — Beginner

Learn:

```text
R Syntax
Variables
Data Types
Operators
Strings
Input / Output
if / else
for
while
Functions
Vectors
Lists
```

Example:

```r
numbers <- c(10, 20, 30)

total <- sum(numbers)

print(total)
```

---

## 🟡 Level 2 — Intermediate

Learn:

```text
Data Frames
Factors
Matrices
Arrays
Dates
Missing Values
File Handling
Packages
Apply Family
dplyr
ggplot2
Statistics
```

Example:

```r
library(dplyr)

result <- students %>%
  filter(score >= 80) %>%
  arrange(desc(score))

print(result)
```

---

## 🟠 Level 3 — Advanced

Learn:

```text
Functional Programming
Object-Oriented Programming
Environments
Error Handling
Database
SQL
APIs
JSON
Testing
R Markdown
Shiny
Machine Learning
```

---

## 🔴 Level 4 — Professional

Learn:

```text
Data Engineering
Machine Learning
Statistical Modeling
Production R
Package Development
CI/CD
Testing
Docker
Cloud Deployment
Database Systems
APIs
Reproducible Research
```

---

# 🧠 R Cheat Sheet

## Variables

```r
x <- 10
```

## Vector

```r
x <- c(1, 2, 3)
```

## List

```r
x <- list(
  name = "Dara",
  age = 20
)
```

## Data Frame

```r
df <- data.frame(
  name = c("Dara", "Sok"),
  score = c(80, 90)
)
```

## Function

```r
add <- function(a, b) {
  a + b
}
```

## Condition

```r
if (x > 10) {
  print("Large")
} else {
  print("Small")
}
```

## Loop

```r
for (i in 1:10) {
  print(i)
}
```

## Filter

```r
df[df$score >= 80, ]
```

## Mean

```r
mean(x)
```

## Sum

```r
sum(x)
```

## Maximum

```r
max(x)
```

## Minimum

```r
min(x)
```

## Missing Values

```r
is.na(x)
```

## Read CSV

```r
read.csv("data.csv")
```

## Write CSV

```r
write.csv(
  df,
  "data.csv",
  row.names = FALSE
)
```

---

# 📁 Recommended GitHub Repository

A good R learning repository can look like:

```text
r-programming/
│
├── README.md
│
├── 01-basics/
│   ├── hello.R
│   ├── variables.R
│   ├── data-types.R
│   └── operators.R
│
├── 02-control-flow/
│   ├── if-else.R
│   ├── for.R
│   └── while.R
│
├── 03-functions/
│   └── functions.R
│
├── 04-data-structures/
│   ├── vectors.R
│   ├── lists.R
│   ├── matrices.R
│   ├── arrays.R
│   └── data-frames.R
│
├── 05-data-analysis/
│   ├── dplyr.R
│   ├── statistics.R
│   └── missing-values.R
│
├── 06-visualization/
│   └── ggplot2.R
│
├── 07-machine-learning/
│   ├── regression.R
│   └── classification.R
│
├── 08-advanced/
│   ├── oop.R
│   ├── environments.R
│   ├── error-handling.R
│   └── functional-programming.R
│
├── projects/
│   ├── beginner/
│   ├── intermediate/
│   └── advanced/
│
└── tests/
    └── testthat/
```

---

# 🚀 Recommended Learning Order

Follow this order:

```text
1. R Syntax
       ↓
2. Variables
       ↓
3. Data Types
       ↓
4. Operators
       ↓
5. Conditions
       ↓
6. Loops
       ↓
7. Functions
       ↓
8. Vectors
       ↓
9. Lists
       ↓
10. Data Frames
       ↓
11. File Handling
       ↓
12. Packages
       ↓
13. dplyr
       ↓
14. ggplot2
       ↓
15. Statistics
       ↓
16. SQL / Databases
       ↓
17. APIs / JSON
       ↓
18. Machine Learning
       ↓
19. R Markdown
       ↓
20. Shiny
       ↓
21. Testing
       ↓
22. Production R
```

---

# 🎯 What Can You Build With R?

After mastering R, you can build:

* 📊 Data Analysis
* 📈 Data Visualization
* 📉 Statistical Models
* 🤖 Machine Learning
* 🧪 Scientific Research
* 📑 Automated Reports
* 🌐 Shiny Web Applications
* 🔌 API Clients
* 🗄️ Database Applications
* 📚 Reproducible Research
* 📦 R Packages
* 🧠 Data Science Pipelines

---

# 📝 Final Notes

## English

The most important thing when learning R is not memorizing every function.

Focus on understanding:

```text
Data
 ↓
Transform
 ↓
Analyze
 ↓
Visualize
 ↓
Model
 ↓
Communicate
```

Practice by building real projects instead of only reading syntax.

## Khmer

ចំណុចសំខាន់ក្នុងការរៀន R គឺ **កុំផ្តោតតែលើការចងចាំ Function ទាំងអស់**។

ត្រូវយល់ពី Workflow៖

```text
Data
 ↓
Transform
 ↓
Analyze
 ↓
Visualize
 ↓
Model
 ↓
Report
```

រៀនដោយបង្កើត Project ពិតៗ នឹងធ្វើឲ្យយល់ R លឿនជាងការអាន Syntax តែប៉ុណ្ណោះ។

---

# ⭐ Summary

R is especially powerful for:

```text
Statistics
Data Analysis
Visualization
Machine Learning
Research
Reporting
```

Start simple:

```r
print("Hello, R!")
```

Then progress toward:

```r
library(dplyr)
library(ggplot2)

result <- students %>%
  filter(score >= 80) %>%
  arrange(desc(score))
```

And eventually:

```r
model <- lm(
  score ~ study_hours + attendance,
  data = students
)

prediction <- predict(
  model,
  newdata = new_student
)
```

**Beginner → Intermediate → Advanced → Professional**

Keep practicing, build projects, test your code, document your work, and use GitHub to track your progress.

---

## 📄 License

This learning material can be used for educational purposes.

---

## 👨‍💻 Author

**Your Name**

GitHub: `https://github.com/your-username`

---

⭐ If this guide helps you learn R, consider giving the repository a star.
