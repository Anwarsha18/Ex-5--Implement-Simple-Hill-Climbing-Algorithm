<h1>ExpNo 5 : Implement Simple Hill Climbing Algorithm</h1> 
<h3>Name:Anwarsha E.M             </h3>
<h3>Register Number:2305001002             </h3>
<H3>Aim:</H3>
<p>Implement Simple Hill Climbing Algorithm and Generate a String by Mutating a Single Character at each iteration </p>
<h2> Theory: </h2>
<p>Hill climbing is a variant of Generate and test in which feedback from test procedure is used to help the generator decide which direction to move in search space.
Feedback is provided in terms of heuristic function
</p>


<h2>Algorithm:</h2>
1. Generate a random initial solution of the same length as the target.
 2. Calculate the score as the ASCII difference between solution and target.
 3. If the score is zero, stop (solution found).
 4. Mutate the solution by changing one random character.
 https://github.com/logesh1326/Ex-5--Implement-Simple-Hill-Climbing-Algorithm/blob/main/README.md
 1/4
06/10/2025, 14:48
 Ex-5--Implement-Simple-Hill-Climbing-Algorithm/README.md at main · logesh1326/Ex-5--Implement-Simple-Hill-Climbing-Al…
 5. Accept the new solution if its score is better, otherwise repeat.

## PROGRAM
```python
 import random, string
 answer = "Artificial Intelligence"
 gen = lambda: [random.choice(string.printable) for _ in range(len(answer))]
 score = lambda s: sum(abs(ord(a)-ord(b)) for a,b in zip(s,answer))
 best = gen()
 while True:
 print("Score:", score(best), "Solution:", "".join(best))
 if score(best) == 0: break
 new = best[:]; new[random.randrange(len(answer))] = random.choice(strin
 if score(new) < score(best): best = new
```


## Input 
Enter the target string: Hi
## Output
```
60 K0
6 Kf
6 Kf
6 Kf
6 Kf
6 Kf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
4 Gf
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
2 Gj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
1 Hj
Final: Hi
```
## Result:
Thus, the program is executed sucessfully.
