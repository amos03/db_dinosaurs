1. Count the number of dinosaurs:

    SELECT COUNT (*) FROM dinos;

    331

2. Find all dinosaurs from Jurassic period:

    SELECT name FROM dinos WHERE period='Jurassic';

    92


3. Find total sum length of all dinosaurs from Cretaceous period:

    SELECT SUM(length) FROM dinos WHERE period='Cretaceous';

    1366.45 m

4. Find all dinosaurs from either Jurassic or Cretaceous period and sort them alphabetically:

    SELECT name FROM dinos WHERE period='Jurassic' OR period='Cretaceous' ORDER BY name;

    310

5. Find all the dinosaurs from the t_order Saurischia that are Herbivorous:

    SELECT name FROM dinos WHERE t_order='Saurischia' AND diet='Herbivorous';

    68

#question on 6 - is there a way to chain it?
6.  Find the shortest dinosaur, and rename it Shortie.

    SELECT MIN(length) FROM dinos;

    0.08

    SELECT id,name, length from dinos where length=0.08;

    160, Liaoxiornis, 0.08

    UPDATE dinos SET name='Shortie' WHERE id=160; 

7. Find the alphabetically first dinosaur

    select name from dinos order by name limit 1;

    Aardonyx

8.  Rename the five longest dinosaurs The Famous Five.

    select id,name,length from dinos where length is not null order by length desc limit 5;
    update dinos set name = 'The Famous Five' where length <=40 and length >= 28;