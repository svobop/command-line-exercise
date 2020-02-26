# Chama Foundation Normal Exam

## Getting Started

- Fork this repository under your own account
- Clone the forked repository to your computer
- Create a `.gitignore` file so generated files won't be committed
- Commit your progress frequently and with descriptive commit messages
- All your answers and solutions should go in this repository

## Keep in mind

- You can use any resource online, but **please work individually**

- **Don't just copy-paste** your answers and solutions,
  use your own words instead

- **Don't push your work** to GitHub until
  your mentor announces that the time is up

## Exercises

### Greatest values in matrices

Write a method which takes two matrices as parameters and returns a new matrix.
The method should compare each element in the input matrices and fill the
returned matrix with the greater values.
You only have to deal with square matrices. 
A square matrix is a matrix with the same number of rows and columns.

Write 2 different test cases for the method.

#### Example 1

Input 1

```text
[
  [2, 1],
  [0, 1]
]
```

Input 2

```text
[
  [0, 3],
  [-1, 1]
]
```

Output

```text
[
  [2, 3],
  [0, 1]
]
```

#### Example 2

Input 1

```text
[
  [-1, 1, 0],
  [0, 1, 0],
  [0, 1, 0]
]
```

Input 2

```text
[
  [0, 0, 0],
  [0, 1, 0],
  [0, 0, 0]
]
```

Output

```text
[
  [0, 1, 0],
  [0, 1, 0],
  [0, 1, 0]
]
```

### Word Frequency

Write a method which can read and parse a file. 
The method must take a frequency as a parameter 
and collects all of the words that appear in
that amount of times in the source file. 
It shall write the selected words into `output.txt`.

If there is no word present with the given frequency
it shall not do anything.

The method must be able to handle the case
if the input file name does not exists.

#### Example

[Example file can be found here.](input.txt)

Input frequency

```text
2
```

The `output.txt` contains this line:

```text
apple, pear, pirate
```

### Zoo

You're going to model a Zoo with animals and workers
and create some interactions between them. 

#### Animal

- It has a name, an age, a gender and

  - a `fedTimes` meaning the number of times the animal got food

We should be able to create animals two ways:

- providing `name`, `age`, `gender` 

- or only providing `name`, when `age` and `gender` will get
  default values `1` and `"unknown"` respectively

- It has an `eat()` method which only increases `fedTimes`.

- It has an `isHungry()` method which returns whether the animal is
  currently hungry.

- It has a `toString()` method which returns information
  about him/her in the format: 

  - "`name` is a `age` years old `gender` animal and was fed `fedTimes` times"

##### Lion

- Lion is **always** hungry.

##### Monkey

- Monkey is **randomly** hungry.

##### Elephant

- Elephant is hungry in **every second occasion**
  when a `Worker` checks on them.

#### Worker

- It has a name and

  - an `animalsToLookAfter` list of containing the animals that they are looking
    after (we should be able to change this field later on)

We should be able to create workers two ways:

- providing `name`, `animalsToLookAfter`

- or only providing `name`, when the `animalsToLookAfter` list
  should be an empty list

It has a `doDailyRoutine()` method which: 

- iterates through the worker's `animalsToLookAfter` list
  and feed them if it is necessary. 

  - first, he/she calls the specific animal's `isHungry()` method

  - and if it returns true, then call the animal's `eat()` method.

## Command line exercise

- Take a look at this directory structure:

```text
homework
 |--math
 |   |--.git
 |   |--calculus
 |   |   |--jacobian_matrix.md
 |   |   └--exercises
 |   |       └--week01_hw.txt
 |   └--geometry
 |       |--week01_hw.txt
 |       └--pithagorean_theorem.md
 └--history
     |--.git
     |--taylor_polynomial.md
     |--history_of_rome.md
     └--history_of_greece.md
```

- Your task is to write commands in the correct order from the directory given below.
- Do it with less commands without chaining them together.
- Assume that the following files are currently in the staging area:
  - `math/calculus/jacobian_matrix.md`
  - `math/geometry/pithagorean_theorem.md`
- Your current directory is `homework/`
  1. Create an `exercises` directory in `math/geometry/`
  1. Move `geometry/week01_hw.txt` to `math/geometry/exercises/`
  1. Move `history/taylor_polynomial.md` to `math/calculus/`
  1. Remove `math/geometry/pithagorean_theorem.md` from the staging area
  1. Rename `math/geometry/pithagorean_theorem.md` to `math/geometry/pythagorean_theorem.md`
  1. Commit all the changes in the `math/` folder

- Solution:

*type your answer here*
