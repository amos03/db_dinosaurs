# Dinosaurs
In this assignment, we'll be looking through a database of dinosaurs, running some SQL queries.

We'll be looking at just one table, the `dinos` table.


## Getting Started
First we need to set up our database from a `.sql` file.


## Columns in the `dinos` table
The `dinos` table contains the following columns:
+ `id` : An autoincrementing unique numerical ID associated with each dinosaur, eg. an ID of 1
+ `name` : The dinosaur's common name, eg. Tyrannosaurus
+ `species` : The dinosaur's species name, eg. Rex
+ `t_order` : The dinosaur's taxonomical order, eg. Saurischia
+ `taxonomy` :  The dinosaur's broader taxonomical classification, eg. Dinosauria, Saurischia, etc.
+ `period` : The period in which the dinosaur lived, eg. Cretaceous
+ `diet` : The dinosaur's diet type, eg. Carnivorous
+ `length` : The dinosaur's length in meters, eg. 12.0 meters

## Questions/Queries
Use SQL queries to complete the following. You can complete them in any order, if you're not sure how to approach one, move on and come back to it:
1. Let's start by figuring out how many dinosaurs we have. Count the number of dinosaurs.
1. We want to open up our own version of Jurassic Park, but this time only with dinosaurs who are actually from the Jurassic period. Find all the dinosaurs from the Jurassic `period`.
1. Jurassic Park was a huge success for us. Now we want to open up a sequel park: Cretaceous Park. This time though, we're  a little more organized, and we want to know how much space all these dinosaurs are going to take up. Find the total sum length of all the dinosaurs from the Cretaceous period.
1. Great news! Our board of investors recently secured us a large island where we can put all the dinosaurs from both Jurassic Park and Cretaceous Park. This new park will be called Juraceous Park, which according to our focus groups really rolls off the tongue. Find all the dinosaurs from either the Jurassic OR Cretaceous periods, and order them by their `species` name alphabetically.
1. Saurischians are the "lizard hipped" order of dinosaurs, and one of the two main branches. All carnivorous dinosaurs are Saurischians, but not all Saurischians are carnivorous. Find all the dinosaurs from the `t_order` Saurischia that are Herbivorous.
1. Dinosaur names are hard to remember. Find the shortest dinosaur, and rename it **Shortie**.
1. It's the first day of Dino School, and we're doing roll call. Find the alphabetically first dinosaur, so we can make sure they're present for class.
1. Rename the five longest dinosaurs **The Famous Five**.

## Data Source
All the data comes from the [Natural History Museum's website](http://www.nhm.ac.uk/discover/dino-directory/name/name-az-all.html). Museums are cool, and you should go to them.
