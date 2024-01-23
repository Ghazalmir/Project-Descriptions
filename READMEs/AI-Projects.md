
# AI Projects | Fall 2023
- Prolog programs solving five important AI problems and techniques, including knowledge representation and reasoning, constraints satisfaction, search, natural language understanding, and planning.

### Contents:
*  [List of Programs](https://github.com/Ghazalmir/project-descriptions/blob/main/READMEs/AI-Projects.md#list-of-programs)
*  [NLP Demo](https://github.com/Ghazalmir/project-descriptions/blob/main/READMEs/AI-Projects.md#nlp-demo)

## List of Programs:
1. Knowledge Bases and Queries: Several knowledge bases and queries written in prolog. 
2. Recursive program finding the Erdos number between people. 
3. Multiple logic puzzles, including crypt-arithmetic puzzles, path finders, and murder mysteries solved using constraint satisfaction.
4. An NLP program that has a knowledge base of albums, artists, and songs, and can answer questions related to individual items as well as the relations between them.
5. Planner programs that plan sequence of actions for a laundry robot and the dining philosophers problem. 

## NLP Demo:
Query 1: 
```
?- what([the, length, of, a, song, by, nick_cave], X).  
X = 204
Yes (0.00s cpu, solution 1, maybe more) ? ;
```
Query 2: 
```
?- what([a, short, smashing_pumpkins, song, released_in, 1979], X). 
X = zero
Yes (0.00s cpu, solution 1, maybe more) ? ;
```
Query 3: 
```
?- what([a, pop, album, by, Bjork, released_before, homogenic], X).  
X = post
Yes (0.00s cpu, solution 1, maybe more) ? ;
```
Query 4: 
```
?- what([the, release_year, of, the, second, song, on, carrie_and_lowell], X).
X = 2015
Yes (0.00s cpu, solution 1, maybe more) ? ;
```
Query 5: 
```
?- what([a, rock, song, released_in, 2019], X).
X = seventeen
Yes (0.00s cpu, solution 1, maybe more) ? ;
```
Query 6: 
```
?- what([an, indie_rock, artist], X).
X = florence_and_the_machine
Yes (0.00s cpu, solution 1, maybe more) ? ;
```
Query 7: 
```
?- what([a, short, folk, song], X).
X = king_of_the_carrot_flowers_pt_1
Yes (0.00s cpu, solution 1, maybe more) ? ;
```
Query 8: 
```
?- what([the, length, of, the, third, song, on, rain_dogs], X).
X = 107
Yes (0.00s cpu, solution 1, maybe more) ? ;
```
Query 9: 
```
?- what([the, length, of, an, old, david_bowie, album], X).
X = 534
Yes (0.02s cpu, solution 1, maybe more) ? ;
```
Query 10: 
```
?- what([the, second, song, on, an, album, released_after, black_holes_and_revelations], X).
X = dear_darkness
Yes (0.00s cpu, solution 1, maybe more) ? ;
```
